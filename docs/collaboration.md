# Collaboration

It's very common for Final Cut Pro editors to have to share libraries between different editors and machines.

When you import a clip via BRAW Toolbox, we create a security-scoped bookmark, that's **specific to the machine you're on**.

This means if you move that Final Cut Pro Library to another machine, Final Cut Pro won't have access to that file, due to sandboxing (which is required by Mac App Store apps).

To solve this issue, if you select a BRAW Toolbox effect in the Final Cut Pro Inspector, you can click the **Global Settings** button to access a **Grant Sandbox Access** menu item.

![Screenshot](static/sandbox.png)

This allows you to easily give BRAW Toolbox read-access to an external hard-drive or network share.

As long as the file path remains consistent between machines (i.e. if you're working off an external hard drive with the same name and folder structure), as long as you grant sandbox access, everything will auto-magically link correctly.

---

### Technical Explanation

Because BRAW Toolbox is sold on the Mac App Store, we have to adhere to very strict security and sandboxing requirements.

The App Sandbox is an access control technology that macOS provides and enforces at the kernel level. The sandbox’s primary function is to restrict what files an application actually has access to.

For example, an App sold on the Mac App Store generally won't have access to any files on your system, unless you explicitly give it permission. This means it can't mess with your user documents or system files.

Whilst this is fantastic for security reasons - it does provide challenges for apps, such as video editors, which is why Final Cut Pro itself isn't actually sandboxed yet.

When you import clips into the BRAW Toolbox Workflow Extension, you are explicitly giving permission to BRAW Toolbox to access those BRAW files.

Everything works great if you're on a single machine. We use a technology called [security-scoped bookmarks](https://developer.apple.com/documentation/professional_video_applications/fcpxml_reference/asset/media-rep/bookmark/enabling_security-scoped_bookmark_and_url_access?language=objc) to allow us to access any files you've given us permission to access at a later time.

However, when it comes to collaboration it gets a bit more tricky, because those bookmarks are specific to the individual machine.

To solve this, we allow you to **Grant Sandbox Access** to specific folders, so that the BRAW Toolbox FxPlug4 can read the files without any issues.

You can always **Reset Sandbox Access** to remove any previously granted permissions. You will need to restart Final Cut Pro for these changes to take affect.
# Installation

### Video

<style>
.video-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
}
.video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>

<div class="video-container">
    <iframe class="video" src="https://www.youtube-nocookie.com/embed/ybuRAGcTPuo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

---

### Instructions

You can download BRAW Toolbox from the Mac App Store.

> [:icon-desktop-download: **Click here to buy on the Mac App Store**](https://apps.apple.com/au/app/braw-toolbox/id6444061549?mt=12)

![Screenshot](static/mac-app-store.png)

When you run it for the first time, you'll be presented with this:

![Screenshot](static/install-01.png)

If it's the first time installing the software, or if there's been an update, you'll be prompted to **Install Motion Templates**, **Install Metadata View** and **Install LUTs**.

> **IMPORTANT:** You should make sure that Final Cut Pro is not running at this point.

Once you click **Install Motion Templates**, you'll be prompted to grant permission to your Movies folder. This is due to macOS's sandboxing, and you'll only need to do this once. Click **OK**.

![Screenshot](static/install-02.png)

You then need to click **Grant Access**:

![Screenshot](static/install-03.png)

Once done, you'll be presented with a successful message:

![Screenshot](static/install-04.png)

After clicking **OK**, the **Install Motion Templates** button will now be disabled, and will instead say **Motion Templates Installed**.

![Screenshot](static/install-05.png)

You should now click the **Install Metadata View** button, and you'll be prompted to grant permission to your ProApps folder. Click **OK** again:

![Screenshot](static/install-07.png)

You need to click the **Grant Access** button:

![Screenshot](static/install-06.png)

Once done, you'll be presented with a successful message:

![Screenshot](static/install-08.png)

The **Install Metadata View** button will now be disabled, and will say **Metadata View Installed**.

![Screenshot](static/install-21.png)

You now need to click the **Install LUTs** button. LUTs are stored in the same root folder as the Metadata View's, so you don't need to grant it permission again.

After clicking the button you'll be presented with a successful message:

![Screenshot](static/install-22.png)

After clicking **OK**, you can now click **Launch Final Cut Pro**, which will close the BRAW Toolbox application and Launch Final Cut Pro.

![Screenshot](static/install-09.png)

> **IMPORTANT:** You should run the BRAW Toolbox application again after each update, to make sure you're using the latest Motion Templates, Metadata View, and LUTs.

Once Final Cut Pro is launched you can access BRAW Toolbox via the **Workflow Extension** button:

![Screenshot](static/install-10.png)

You can also access it via the **Window > Extensions > BRAW Toolbox** menu item:

![Screenshot](static/install-11.png)

When you click either of those options it opens the BRAW Toolbox Workflow Extension:

![Screenshot](static/install-12.png)

To import some BRAW clips, click the **Import BRAW Files** button and select some BRAW clips.

> **TIP:** You can also drag-and-drop BRAW files from Finder to the File List.

![Screenshot](static/install-13.png)

You can now adjust all the metadata as required. There are tools for easily copy and pasting RAW parameters between clips, as well as saving Metadata Presets.

Whilst BRAW Toolbox can play back BRAW video files natively, to handle audio, it "extracts" the audio prior to sending to Final Cut Pro. You should press the **Choose Audio Folder** button to select the destination folder for these audio files.

Once you've tweaked any metadata settings, you can press the **Prepare BRAW Files** to get everything ready for Final Cut Pro.

> **NOTE:** If you haven't already pressed the **Choose Audio Folder**, it'll prompt you regardless the first time you click **Prepare BRAW Files**.

Whilst it's processing you'll see this:

![Screenshot](static/install-23.png)

Once it's processed, you'll get the below alert explaining what to do next.

> **TIP:** You can tick **Do not show this message again** to speed things up next time (and press **Reset Dialog Warning** via the Settings button if you want to bring this back).

![Screenshot](static/install-14.png)

Essentially, you need to drag this green button:

![Screenshot](static/install-15.png)

...to your Final Cut Pro **Library**.

> **IMPORTANT:** You need to drag to a **Library** - not an **Event** or a **Project**, otherwise nothing will happen.

This will create a new Keyword Collection with your BRAW clips:

![Screenshot](static/install-16.png)

You can now drag these Synchronised Clips into a Project/Timeline and start editing, as you would normal video clips.

> **IMPORTANT:** Whilst you can modify the RAW parameters, as explained next, you shouldn't ever "cut" or change the timing of the Generator contained within the Synchronised Clip.

To modify the metadata of a BRAW clip, you can double click on one of the synchronised clips, click on the black video clip, then access the BRAW Toolbox effect in the Effects section of the Inspector:

![Screenshot](static/install-17.png)

Click the **Show Parameters** button to show the parameters. You'll only have to do this once per clip, as Final Cut Pro will remember it's been opened.

![Screenshot](static/install-18.png)

Frame Metadata and Custom Gamma Controls are key-frame-able.

> **TIP:** You can only access Custom Gamma Controls if you have the **Blackmagic Design Custom** gamma parameter selected.

You can now edit BRAW files like any other camera media in Final Cut Pro. Woohoo!


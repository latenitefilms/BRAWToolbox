# Troubleshooting

### Why can't I adjust the Custom Gamma Controls?

You can only adjust the Custom Gamma Controls if you select the **Blackmagic Design Custom** Gamma option.

---

### Why can't I adjust the RAW metadata within Final Cut Pro?

You absolutely can - that's the big benefit of BRAW Toolbox. You can even keyframe the ISO, Exposure, Color Temp, Tint and all the Custom Gamma Controls.

As explained in the [Installation](https://brawtoolbox.io/installation/) section, you can only access the BRAW Toolbox effect from WITHIN the Synchronised Clip or Multicam Clip.

Why this is the case, is explained in more detail in the [How does it work](https://brawtoolbox.io/faq/#how-does-it-work) FAQ.

For example, if you have imported the below clips as Synchronised Clips:

![Screenshot](static/access-raw-01.png)

If you then double click on one of those clips in the Browser, it will open the clip in the timeline.

You'll see a black clip on the Primary Storyline, which is your BRAW footage. Click that clip, then in the Effects Inspector you can access the BRAW Toolbox controls.

![Screenshot](static/access-raw-02.png)

The same logic applies to clips already in the project/timeline. If it's a Synchronised Clip, you can double click on it to access the clip that contains the BRAW Toolbox effect.

Keep in mind that when you import a Synchronised Clip from the Browser to a Project, Final Cut Pro creates a new instance of that clip - so if you modify the RAW controls in the browser instance, it won't update in the individual timeline instances.

This is standard Final Cut Pro behaviour - and nothing to do with BRAW Toolbox.

However, if you've ticked **Create Multicam Clips** within the **Settings** button in the BRAW Toolbox Workflow Extension, it will create Synchronised Clips WITHIN a Multicam Clip, so that you can modify the Synchronised Clip, and any changes will ripple across all instances of the Multicam Clip.

![Screenshot](static/access-raw-03.png)

---

### BRAW Toolbox Workflow Extension doesn't appear in Final Cut Pro?

Sometimes macOS can be a bit temperamental with System Extensions, including Workflow Extensions.

If you can't see BRAW Toolbox in the Workflow Extension button or menu bar, you can try:

1. Restart your Mac.
2. [Trash Final Cut Pro Preferences](https://support.apple.com/en-au/HT203477) by holding down COMMAND + OPTION when launching Final Cut Pro.
3. Delete Final Cut Pro and reinstall it from the App Store.

If none of those things fix it, please post an issue [here](https://github.com/latenitefilms/BRAWToolbox/issues).

---

### "The effect ID is invalid"

If you see an error message saying "The effect ID is invalid" when trying to import from the BRAW Toolbox Workflow Extension to Final Cut Pro, it means that the FxPlug4 Filter is not being detected by Final Cut Pro.

You can try:

1. Restart your Mac.
2. [Trash Final Cut Pro Preferences](https://support.apple.com/en-au/HT203477) by holding down COMMAND + OPTION when launching Final Cut Pro.
3. Delete Final Cut Pro and reinstall it from the App Store.

If none of those things fix it, please post an issue [here](https://github.com/latenitefilms/BRAWToolbox/issues).

---

### Bad Frames in the Final Cut Pro Browser

In rare instances in the Final Cut Pro Browser you might see black frames, or red error message frames in the thumbnails of BRAW Toolbox clips.

![Screenshot](static/bad-frame.png)

This is generally because Final Cut Pro has an outdated thumbnail cache, or something went wrong when creating the thumbnails.

This is a Final Cut Pro bug, rather than anything specifically wrong with BRAW Toolbox.

In Filmstrip mode, try changing the time slider from **All** to **½s** and see if that kicks Final Cut Pro back into gear.

![Screenshot](static/browser.png)

If all the frames look correctly in **½s** view, but incorrect when you change back to **All** it most likely means your thumbnail cache is corrupt, and Final Cut Pro isn't updating it.

To try and fix this, you can close Final Cut Pro, right click on the Library in Finder and select **Show Package Contents**, then within the problem Event folder, go into the **Render Files** folder, and delete the **Thumbnail Media** folder.

When you start Final Cut Pro again, this will force it to re-generate the thumbnails, and hopefully this time, it works correctly.

![Screenshot](static/thumbnails.png)

---

## Failed to install Metadata View

In rare instances you might run into problems installing the Metadata View.

![Screenshot](static/failed-to-install-metadata-view.png)

Please close BRAW Toolbox, then open the `Terminal` app, then execute the following command:

```
/usr/bin/defaults delete com.latenitefilms.BRAWToolbox
```

This will delete all the BRAW Toolbox preferences.

Try running the BRAW Toolbox application again, and be careful to follow [these exact steps](https://brawtoolbox.io/installation/), making sure you don't accidentally change the folders when prompted to **Grant Permission**.

If this still doesn't work, please [post an issue](https://github.com/latenitefilms/brawtoolbox/issues) and we'll try and resolve your specific problem.

---

### I've run into a bug. Where can I find the log files?

You can find the log files here:

`/Users/YOUR-USER-NAME/Library/Group Containers/A5HDJTY9X5.com.latenitefilms.BRAWToolbox/Library/Application Support/`

You can find any crash reports here:

`/Users/YOUR-USER-NAME/Library/Logs/DiagnosticReports`

You can send the files to LateNite Films [here](https://latenitefilms.digitalpigeon.com).
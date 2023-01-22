# Frequently Asked Questions

### Where can I find some sample BRAW clips?

There are heaps of awesome clips to test with on the Blackmagic Website:

- [Blackmagic Pocket Cinema Camera Gallery](https://www.blackmagicdesign.com/au/products/blackmagicpocketcinemacamera/gallery)
- [Blackmagic URSA Mini Gallery](https://www.blackmagicdesign.com/au/products/blackmagicursaminipro/gallery)

---

### Does BRAW Toolbox work with Sync-N-Link?

Yes, BRAW Toolbox is compatible with **Sync-N-Link v1.1.4** on the Mac App Store.

You should use Synchronised Clips in BRAW Toolbox, and it can combine multiple clips with location audio into a multicam.

---

### BRAW Toolbox Workflow Extension doesn't appear in Final Cut Pro?

Sometimes macOS can be a bit temperamental with System Extensions, including Workflow Extensions.

If you can't see BRAW Toolbox in the Workflow Extension button or menu bar, you can try:

1. Restart your Mac.
2. [Trash Final Cut Pro Preferences](https://support.apple.com/en-au/HT203477) by holding down COMMAND + OPTION when launching Final Cut Pro.
3. Delete Final Cut Pro and reinstall it from the App Store.

If none of those things fix it, please post an issue [here](https://github.com/latenitefilms/BRAWToolbox/issues).

---

### I don't like Synchronised Clips. Can I import a Multicam clips instead?

Yes, you can click the **Settings** button (the gear icon, next to "Remove All") to **Create Multicam Clips** instead.

Please note that this doesn't sync multiple BRAW files together - it just creates a single Multicam Clip for each BRAW file.

You'll still need to use something like [Sync-N-Link](https://apps.apple.com/us/app/sync-n-link-x/id517599985?mt=12) if you want to sync BRAW files with external audio.

![Screenshot](static/install-20.png)

---

### Why can't I adjust the Custom Gamma Controls?

You can only adjust the Custom Gamma Controls if you select the **Blackmagic Design Custom** Gamma option.

---

### Can I stabilise clips using the Gyroscope Data within the BRAW file?

Yes, you can combine BRAW Toolbox with [Gyroflow Toolbox](https://github.com/latenitefilms/GyroflowToolbox) - simply apply the Gyroflow Toolbox effect to the video layer inside your Synchronised or Multicam clip.

---

### Is BRAW Toolbox Open Source?

Currently the source code for BRAW Toolbox is private, however we may release it under a MIT License at a later date after it's been publicly released on the Mac App Store.

---

### I've run into a bug. Where can I find the log files?

You can find the log files here:

`/Users/YOUR-USER-NAME/Library/Group Containers/A5HDJTY9X5.com.latenitefilms.BRAWToolbox/Library/Application Support/`

You can find any crash reports here:

`/Users/YOUR-USER-NAME/Library/Logs/DiagnosticReports`
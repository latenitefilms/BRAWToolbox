<img src="https://github.com/latenitefilms/BRAWToolbox/raw/main/Documentation/BRAWToolbox.png" align="right" width="15%" height="15%" />

# BRAW Toolbox

BRAW Toolbox allows you to import Blackmagic RAW files directly into Final Cut Pro without transcoding.

---

## Download

BRAW Toolbox is currently in **public beta**. If all goes to plan, we intend to release on the Mac App Store in late January.

You can currently access the latest build on Apple's TestFlight [here](https://testflight.apple.com/join/dbWjWl8e).

TestFlight requires macOS Monterey or later.

---

## Help & Support

If you run into any issues, bugs or crashes, you can post an issue [here](https://github.com/latenitefilms/BRAWToolbox/issues).

If you have any general questions or feedback, you can discuss [here](https://github.com/latenitefilms/BRAWToolbox/discussions).

---

## Release Notes

### 1.0.0 (15) - Public Beta 2

**Important:**
- Due to major changes, this beta is **not** compatible with the previous beta, so you should re-create any test Final Cut Pro libraries.
- If you have installed and used the previous beta, you will need to install the new Motion Template and Metadata View, prior to launching Final Cut Pro.

**Improvements:**
- The BRAW Toolbox Motion Template has been completely redesigned to be a lot faster and easier to use. We have removed all the override controls. It now only shows the parameters that you can control (i.e. if your camera doesn't allow manipulating the ISO, we no longer show this parameter).
- We added a "Global Settings" button to the Motion Template in the Final Cut Pro Inspector, so that you can force a Decode Quality across all clips. This is useful if you have clips with different Decode Quality settings, but you want to export at the highest quality.
- We now populate the "Ingest Date" (aka "Date Imported" in Final Cut Pro) metadata field. Thanks for suggesting @tangierc!
- The Workflow Extension has been redesigned. The checkboxes no longer act as "overrides", but instead allow you to select which parameters you want to copy, paste, etc.
- The buttons at the bottom of the Workflow Extension Inspector (Copy, Paste, etc.) now all work.
- All the parameters in the Workflow Extension should now flow into Final Cut Pro.
- All the parameters in the Final Cut Pro Inspector should now work and update correctly. Thanks for reporting @markspen!
- We now display an error message if you press "Show Parameters" with no BRAW file loaded.
- We no longer hide the Workflow Extension player slider when playing, and now update its value during playback. Thanks for suggesting @JW144754!
- The Viewer in the Workflow Extension is now resizable. Thanks for suggesting @JW144754!
- The main application now only asks for permissions to your Movies folder and Application Support folder once.
- All the individual open/save dialog boxes now remember their own last opened path.
- The "Convert PROJECT to Resolve Friendly FCPXML" Toolbox now works.

**Changes:**
- We now write log files to `~/Library/Group Containers/A5HDJTY9X5.com.latenitefilms.BRAWToolbox/Library/Application Support/` folder, for easier debugging.
- BRAW Toolbox will now run on macOS Big Sur and above.

**Bug Fixes:**
- Fixed various memory leaks.
- Fixed a bug which prevented the correct Decode Quality from being used. Thanks for reporting @JW144754!
- Fixed a bug in the ISO parameter.
- Error messages in Final Cut Pro now show the correct icon.
- Added some missing Metadata Definition labels.

**Known Issues:**
- The "Relink Unliked BRAW Clips within an EVENT" Toolbox is not yet implemented.
- The "Convert BRAW clips to MOV's within an EVENT" Toolbox is not yet implemented.

### 1.0.0 (14) - Public Beta 1

This is the first public beta of BRAW Toolbox. Woohoo!

This build is very much a work-in-progress, and doesn’t contain all our latest code (due to delays and complexity of getting things approved by Apple’s App Review). However, now that the first beta is out, we hope to be able to push out new builds much more quickly in the New Year, as we work towards a public release.

The main area we’d like to test at this point is making sure that all machines can successfully import and playback BRAW files. Currently we’ve been primarily testing on MacBook Pro’s (16-inch, 2021, M1 Max, 64GB RAM) running macOS Monterey and Final Cut Pro 10.6.5. We're particularly interested to see how things work on MacPro's with multiple GPUs.

The Workflow Extension is currently very incomplete. All of the parameters from Color Science Version onwards currently don’t come across to Final Cut Pro. The buttons at the bottom of the parameters also don’t currently do anything. The Toolbox currently doesn’t do anything.

Happy testing!

---

## Installation

When you first launch the BRAW Toolbox application, you'll need to press the **Install Motion Template** button, which will install the "BRAW Toolbox" effect into Final Cut Pro. You'll then need to press the **Install Metadata View**, which will install the Custom Metadata View. Once this is done you can close the BRAW Toolbox application and launch Final Cut Pro.

During the beta testing stage, you should run the BRAW Toolbox application after each update to see if you need to re-install either the Motion Template or the Metadata View.

From within Final Cut Pro you can access the BRAW Toolbox via the Workflow Extension toolbar icon (or the "Window > Extensions" menubar item).

In the Workflow Extension, you can import BRAW files and adjust their metadata, prior to importing the files into Final Cut Pro.

Whilst BRAW Toolbox can play back BRAW video files natively, to handle audio, it "extracts" the audio prior to sending to Final Cut Pro. You should press the "Choose Audio Folder" button to select the destination folder for these audio files. Once you've tweaked any metadata settings, you can press the "Prepare BRAW Files" button to extract the audio. Once that's done, you can drag the event icon from the Workflow Extension to your Final Cut Pro Event. This will create a new Event which contains your BRAW clips. The BRAW clips will come across as Synchronised Clips. If you double click on a Synchronised Clip, and click on the video clip, you can adjust all the BRAW metadata parameters within the Video Inspector.

Whilst we recommend always using the Workflow Extension to import BRAW files, you can do it manually by applying the BRAW Toolbox effect to any clip, such as a Generator. You can also access the BRAW Toolbox effect as a "filter" within Apple Motion.
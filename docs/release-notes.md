# Release Notes

### 1.0.0 (26) - Public Beta 13

**Released:**
- 17th January 2023

**Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**Improvements:**
- We now display the current timecode value of the selected clip in the Workflow Extension player in the bottom right corner.
- Added additional metadata columns to the file list in the Workflow Extension. You can now right-click on the columns to enable/disable columns.
- Added a **Convert PROJECT to Resolve Friendly FCPXML (via CP)** Toolbox item, which sends the FCPXML to CommandPost after processing. This is useful if you have BRAW clips and you also need CommandPost's Sony Timecode Repair Toolbox prior to sending to DaVinci Resolve. Thanks for suggesting [George Elias](https://twitter.com/gwphotographe)!
- We now remember the last Toolbox item when you close and re-open the Workflow Extension.
- Added a **Do not show this message again** button to the **Convert PROJECT to Resolve Friendly FCPXML** Toolbox success popup message.
- The default image in the Workflow Extension Player has been changed to make it look a bit nicer.

**Bug Fix:**
- Fixed a bug where the player controls weren't always updating the player content correctly.
- Fixed a bug where if you didn't have any BRAW clips selected, certain parameters would still be accessible.

---

### 1.0.0 (25) - Public Beta 12

**Released:**
- 16th January 2023

**Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**Bug Fix:**
- Fixed a bug in the **Convert PROJECT to Resolve Friendly FCPXML** Toolbox, where the Toolbox would fail if there's any BRAW Toolbox clips in the project/timeline where there hasn't been any BRAW files loaded. Thanks for discovering Kevin Luk!

---

### 1.0.0 (24) - Public Beta 11

**Released:**
- 16th January 2023

**Note:**
- The Motion Templates have been updated in this release.

**Improvements:**
- After clicking **Prepare BRAW Files**, once complete, the draggable FCPXML icon now turns green. This is useful if you have selected **Do not show this message again**, on the **Successfully Processed** popup. Thanks for suggesting Chris Gosling!

**Bug Fix:**
- Fixed a bug in the **DWG Intermediate to Rec. 2020 PQ** Motion Template. Thanks for reporting Jamie Lejeune!

---

### 1.0.0 (23) - Public Beta 10

**Released:**
- 15th January 2023

**Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**Improvements:**
- Added a checkbox that says "Do not show this message again" to the bottom of various messages in the Workflow Extension. You can "Reset Dialog Warnings" via the Settings button. Thanks for suggesting Chris Gosling!
- We're now using FxPlug v4.2.5 (instead of v4.2.4). According to the release notes this should have improved reconnection with plug-ins after a memory jetsam event and improved the speed of reconnection with plug-ins after a crash, or plug-in process suspension by macOS.

**Bug Fix:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (22) - Public Beta 9

**Released:**
- 15th January 2023

**Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**Bug Fix:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (21) - Public Beta 8

**Released:**
- 15th January 2023

**Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**Bug Fix:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (20) - Public Beta 7

**Released:**
- 14th January 2023

**Note:**
- The Motion Templates and Metadata View has been updated in this release. You now also need to install the LUTs when you first run the application (used for HDR).
- We no longer store the Metadata View in the `/Library/Application Support/ProApps/Metadata Definitions/` folder - it's now stored in the user library. You should **manually** delete the `BRAW Toolbox.plist` file in this folder if you've used earlier beta builds.

**Improvements:**
- We've re-designed the Metal pipeline, to HOPEFULLY improve performance on older 2013 Mac Pro's with Dual AMD FirePro D500. These changes MIGHT also improve performance on other systems. Thanks for reporting [@tangierc](https://github.com/tangierc)!
- Thanks to the amazing Marc Bach & Jamie Lejeune, we've redesigned how BRAW Toolbox handles HDR content, so it better matches DaVinci Resolve.
- There are now **Color Space** settings in the **Settings** button (the gear icon) within the Workflow Extension. This controls the Player in the Workflow Extension, and also the settings of the Synchronised Clips or Multicam Clips that are imported into Final Cut Pro.
- If you select the **DaVinci Wide Gamut** Color Space/Gamut and **DaVinci Intermediate** Gamma, there's now also an option within the Settings button to enable a special LUT which gets applied within Final Cut Pro (the effect of the LUT isn't visible in the Workflow Extension) to better match DaVinci Resolve. Using this option with a **Wide Gamut HDR - Rec. 2020 PQ** Library & Project is the recommended way to grade HDR BRAW in Final Cut Pro.
- Added settings to select the **Default Decode Quality**.
- The thumbnails for the Effects within Final Cut Pro have been improved so they look nicer.
- The BRAW Toolbox Metadata View now contains additional built-in fields, that are used by Sync-N-Link.

**Bug Fixes:**
- We now remember the Audio Folder if you click **Prepare BRAW Files** before clicking **Choose Audio Folder**.
- Fixed a regression which broke the **Remove All** button.

---

### 1.0.0 (19) - Public Beta 6

**Released:**
- 7th January 2023

**Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**Improvements:**
- Added a **Settings** button (the gear icon), with the ability to **Create Multicam Clips** instead of Synchronised Clips. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- **Convert PROJECT to Resolve Friendly FCPXML** has been improved so that Audio Attributes and Rate Conform settings come across more accurately between Final Cut Pro and DaVinci Resolve. Thanks for reporting [@markspen](https://github.com/markspen)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to **Rec.2100 ST2084 (PQ)** in the Workflow Extension, we'll use the **Rec. 2020 PQ** setting for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to **Rec.2100 Hybrid Log Gamma** in the Workflow Extension, we'll use the **Rec. 2020 HLG** setting for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to something other than PQ or HLG in the Workflow Extension, we'll use the **Rec. 2020** setting  for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!

**Bug Fixes:**
- Fixed a bug where clicking the **Gamma** checkbox, and then **Apply Checked To All** would fail.

---

### 1.0.0 (18) - Public Beta 5

**Released:**
- 6th January 2023

**Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**Bug Fix:**
- Fixed a bug where we were releasing `copiedParameters` incorrectly when the Workflow Extension was closed.

---

### 1.0.0 (17) - Public Beta 4

**Released:**
- 6th January 2023

**Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**Improvements:**
- Renamed the **Clear BRAW Files** button to **Remove All** and added a **Remove Selected** button. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- Added ability to drag-and-drop BRAW files from Finder into the BRAW Toolbox Workflow Extension. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- Left-aligned the buttons in the Final Cut Pro Inspector so they don't exhibit any weird UI glitches. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- Sliders in the Workflow Extension are now all continuous, and update the Viewer instantly.
- Added Tooltips to the Workflow Extension.

---

### 1.0.0 (16) - Public Beta 3

**Released:**
- 5th January 2023

**Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**Bug Fixes:**
- Fixed a weird bug which caused the **Preparing BRAW Files** to never close on Intel Mac's (but worked fine on Apple Silicon Mac's). Thanks for reporting [George Elias](https://twitter.com/gwphotographe)!
- Increased the Workflow Extension height by a tiny amount so it looks better on Intel Mac's.

---

### 1.0.0 (15) - Public Beta 2

**Released:**
- 5th January 2023

**Important:**
- Due to major changes, this beta is **not** compatible with the previous beta, so you should re-create any test Final Cut Pro libraries.
- If you have installed and used the previous beta, you will need to install the new Motion Template and Metadata View, prior to launching Final Cut Pro.

**Improvements:**
- The BRAW Toolbox Motion Template has been completely redesigned to be a lot faster and easier to use. We have removed all the override controls. It now only shows the parameters that you can control (i.e. if your camera doesn't allow manipulating the ISO, we no longer show this parameter).
- We added a **Global Settings** button to the Motion Template in the Final Cut Pro Inspector, so that you can force a Decode Quality across all clips. This is useful if you have clips with different Decode Quality settings, but you want to export at the highest quality.
- We now populate the **Ingest Date** (aka "Date Imported" in Final Cut Pro) metadata field. Thanks for suggesting [@tangierc](https://github.com/tangierc)!
- The Workflow Extension has been redesigned. The checkboxes no longer act as "overrides", but instead allow you to select which parameters you want to copy, paste, etc.
- The buttons at the bottom of the Workflow Extension Inspector (Copy, Paste, etc.) now all work.
- All the parameters in the Workflow Extension should now flow into Final Cut Pro.
- All the parameters in the Final Cut Pro Inspector should now work and update correctly. Thanks for reporting [@markspen](https://github.com/markspen)!
- We now display an error message if you press **Show Parameters** with no BRAW file loaded.
- We no longer hide the Workflow Extension player slider when playing, and now update its value during playback. Thanks for suggesting @JW144754!
- The Viewer in the Workflow Extension is now resizable. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- The main application now only asks for permissions to your Movies folder and Application Support folder once.
- All the individual open/save dialog boxes now remember their own last opened path.
- The **Convert PROJECT to Resolve Friendly FCPXML** Toolbox now works.
- We've added a loading screen when BRAW Toolbox is Preparing BRAW Files. Thanks for suggesting [@tangierc](https://github.com/tangierc)!

**Changes:**
- We now write log files to `/Users/YOUR-USER-NAME/Library/Group Containers/A5HDJTY9X5.com.latenitefilms.BRAWToolbox/Library/Application Support/` folder, for easier debugging.
- BRAW Toolbox will now run on macOS Big Sur and above.

**Bug Fixes:**
- Fixed various memory leaks.
- Fixed a bug which prevented the correct Decode Quality from being used. Thanks for reporting [@JW144754](https://github.com/JW144754)!
- Fixed a bug in the ISO parameter.
- Error messages in Final Cut Pro now show the correct icon.
- Added some missing Metadata Definition labels.

---

### 1.0.0 (14) - Public Beta 1

**Released:**
- 23rd December 2022

This is the first public beta of BRAW Toolbox. Woohoo!

This build is very much a work-in-progress, and doesn’t contain all our latest code (due to delays and complexity of getting things approved by Apple’s App Review). However, now that the first beta is out, we hope to be able to push out new builds much more quickly in the New Year, as we work towards a public release.

The main area we’d like to test at this point is making sure that all machines can successfully import and playback BRAW files. Currently we’ve been primarily testing on MacBook Pro’s (16-inch, 2021, M1 Max, 64GB RAM) running macOS Monterey and Final Cut Pro 10.6.5. We're particularly interested to see how things work on MacPro's with multiple GPUs.

The Workflow Extension is currently very incomplete. All of the parameters from Color Science Version onwards currently don’t come across to Final Cut Pro. The buttons at the bottom of the parameters also don’t currently do anything. The Toolbox currently doesn’t do anything.

Happy testing!
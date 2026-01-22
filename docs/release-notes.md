# Release Notes

### 1.4.8 (78)

**🎉 Released:**
- Thursday 22nd January 2026

**🔨 Improvements:**
- Updated the BRAW Toolbox application icon for macOS 26 Tahoe. Thanks Matthew Skiles!

---

### 1.4.7 (77)

**🎉 Released:**
- Friday 7th November 2025

**🔨 Improvements:**
- Added support for Blackmagic PYXIS 12K.
- Added support for Leica SL3-S, Sony FX3 and Sony FX30 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.6.1 to v5.1.

---

### 1.4.6 (76)

**🎉 Released:**
- Tuesday 15th July 2025

**🔨 Improvements:**
- Added support for Panasonic LUMIX S1RII Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.6 to v4.6.1.

---

### 1.4.5 (75)

**🎉 Released:**
- Saturday 14th June 2025

**🔨 Improvements:**
- We've improved how we render error messages in BRAW Toolbox. HUGE thank you to Darrin Cardani at Apple and Gabriele de Simone at FxFactory for all your ongoing help, assistance, genius and support (and for putting up with my crazy questions)!
- Added support for Panasonic LUMIX S1II and S1IIE Blackmagic RAW clips.
- Improved performance for URSA Cine 12K LF and URSA Cine 17K 65 clips.
- Updated from Blackmagic RAW SDK v4.5 to v4.6.
- Updated from FxPlug v4.3.2 to v4.3.3.

---

### 1.4.4 (74)

**🎉 Released:**
- Thursday 3rd April 2025

**🔨 Improvements:**
- Added support for Blackmagic URSA Cine 17K 65.
- Added support for updated Constant Quality record settings on URSA Cine.
- Added support for Panasonic UB-50 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.4 to v4.5.
- Updated from FxPlug v4.3.1 to v4.3.2.

---

### 1.4.3 (73)

**🎉 Released:**
- Thursday 30th January 2025

**🔨 Improvements:**
- Added support for Panasonic UB10 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.3.1 to v4.4.

**🐞 Bug Fix:**
- Fixed a regression where the Toolbox drop zone failed to work properly in older versions of Final Cut Pro.

---

### 1.4.2 (72)

**🎉 Released:**
- Monday 9th December 2024

**🐞 Bug Fixes:**
- Fixed a bug where the Toolbox drop zone failed to work properly in Final Cut Pro 11 due to depreciated FCPXML versions. Thanks for reporting Alex Sofonea!
- Fixed a bug where the "Check All/Uncheck All" button in the Workflow Extension didn't work correctly. Thanks for reporting Mathew Welsh!

---

### 1.4.1 (71)

**🎉 Released:**
- Sunday 17th November 2024

**🔨 Improvements:**
- Updated from Blackmagic RAW SDK v4.3 to v4.3.1.
- Updated from FxPlug v4.3 to v4.3.1.
- Improved Blackmagic RAW SDK stability with simultaneous decodes.

---

### 1.4.0 (70)

**🎉 Released:**
- Saturday 19th October 2024

**🔨 Improvements:**
- Added support for Fujifilm X-M5 Blackmagic RAW clips.
- Added support for Panasonic S5D Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.2 to v4.3.

**🐞 Bug Fix:**
- Fixed a bug when using macOS Sequoia where the hero BRAW Toolbox application would fail to set the correct folders when trying to grant sandbox permissions when first setting up BRAW Toolbox. For example, it would default to the user's "Documents" folders, rather than the user's "Movies" folder and the user's "ProApps" folder. Thanks for reporting Karl Winegardner, Robbie Myers, Jens Pluimes & Edwin van W!
- Re-designed how we render error messages in Final Cut Pro using Core Image and Metal. Hopefully this will fix random crashes some users are seeing on older versions of Final Cut Pro running on older Intel machines.

---

### 1.3.11 (69)

**🎉 Released:**
- Wednesday 24th July 2024

**🔨 Improvements:**
- Added support for Blackmagic PYXIS 6K.
- Added support for Fujifilm X-T50 Blackmagic RAW clips.
- Improves support for Blackmagic URSA Cine 12K LF.
- Updated from Blackmagic RAW SDK v4.1 to v4.2.

---

### 1.3.10 (68)

**🎉 Released:**
- Friday 28th June 2024

**🔨 Improvements:**
- Added support for Fujifilm GFX100S II Blackmagic RAW clips.
- Added support for Panasonic GH7 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v4.0 to v4.1.

---

### 1.3.9 (67)

**🎉 Released:**
- Tuesday 22nd June 2024

**🔨 Improvements:**
- Updated from FxPlug v4.2.9 to FxPlug v4.3

---

### 1.3.8 (66)

**🎉 Released:**
- Tuesday 23rd April 2024

**🔨 Improvements:**
- Added support for Blackmagic URSA Cine 12K LF.
- Updated from Blackmagic RAW SDK v3.6.1 to v4.0.

**🐞 Bug Fix:**
- When clicking "Prepare BRAW Files", you'll now get an error message if the Audio Folder is currently in the Trash. Thanks for reporting Mark Terry!

---

### 1.3.7 (65)

**🎉 Released:**
- Tuesday 19th December 2023

**🐞 Bug Fix:**
- Fixed white balance control for Panasonic GH5S and BGH1 Blackmagic RAW clips.

**🔨 Improvements:**
- Updated from Blackmagic RAW SDK v3.6 to v3.6.1.

---

### 1.3.6 (64)

**🎉 Released:**
- Thursday 7th December 2023

**🐞 Bug Fix:**
- Fixed a potential crash that we've been trying to solve for ages. On SOME systems (specifically systems with [Mac2 family GPUs](https://developer.apple.com/metal/Metal-Feature-Set-Tables.pdf)), Apple's Metal Framework would generate a Metal Texture that the Metal Performance Shader in the Mac couldn't actually work with, causing a crash deep within Apple's code. It was very hard to reproduce, as it only happened on certain systems - and none of ours. HUGE thank you to Apple Developer Technical Support, the Final Cut Pro Team, AdrianEddy and Warren Moore for all their constant and on-going help, assistance, guidance, patience and support!

---

### 1.3.5 (63)

**🎉 Released:**
- Tuesday 5th December 2023

**🔨 Improvements:**
- Added support for Blackmagic Micro Studio Camera 4K G2.
- Added support for Panasonic Lumix G9II Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v3.4 to v3.6.
- Updated from FxPlug v4.2.8 to v4.2.9.

**🐞 Bug Fix:**
- Fixed a potential crash when pressing the **Remove Selected** button in the Workflow Extension.

---

### 1.3.4 (62)

**🎉 Released:**
- Tuesday 14th November 2023

**🐞 Bug Fix:**
- In the previous BRAW Toolbox v1.3.3 (59) release, we made some major under-the-hood changes to improve playback performance (such as only using one shared instance of the BRAW SDK Factory). Unfortunately however, those changes resulted in the BRAW SDK not releasing used threads correctly, and as the thread count grew, eventually the BRAW Toolbox Renderer would stop working correctly in Final Cut Pro. This would only really happen on older machines, and Libraries with hundreds of BRAW clips. We've now reverted back to how we were doing things in v1.3.2 (57) and earlier, with some additional checks and protections. We will continue to research and explore ways we can improve playback performance, so that the export times of timelines with BRAW clips in Final Cut Pro get closer to what you see in DaVinci Resolve.

---

### 1.3.3 (59)

**🎉 Released:**
- Saturday 7th October 2023

**🔨 Improvements:**
- General playback performance improvements.
- Updated from FxPlug 4.2.7 to FxPlug 4.2.8.
- The wrapper application now quits when you close the main window.

---

### 1.3.2 (57)

**🎉 Released:**
- Saturday 16th September 2023

**🐞 Bug Fix:**
- Fixed a crash that could occur when a BRAW file has audio longer than the vision. Thanks for reporting Albert Planella!

---

### 1.3.1 (56)

**🎉 Released:**
- Friday 15th September 2023

**🔨 Improvements:**
- Added support for Blackmagic Cinema Camera 6K.
- Added support for Fujifilm GFX100 II Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v3.3 to v3.4.

---

### 1.3.0 (55)

**🎉 Released:**
- Tuesday 11th July 2023

**🔨 Improvements:**
- Added support for Panasonic Lumix GH6 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v3.2 to v3.3.

---

### 1.2.2 (54)

**🎉 Released:**
- Thursday 22nd June 2023

**🐞 Bug Fix:**
- We've added a bunch of additional checks to the FxPlug4 Renderer, to ensure that all objects received from the Blackmagic RAW SDK are valid and correct to avoid any potential crashes due to referencing null pointers. Thanks for reporting Dominik Radecki! Big thanks to the Blackmagic RAW team and Final Cut Pro team for all their help and support!

---

### 1.2.1 (53)

**🎉 Released:**
- Thursday 22nd June 2023

**🐞 Bug Fix:**
- The Workflow Extension now gracefully aborts (instead of crashing), and shows an error message if a BRAW clip is corrupt, and the metadata can't be read. Thanks for reporting Dominik Radecki!

---

### 1.2.0 (52)

**🎉 Released:**
- Thursday 15th June 2023

**🔨 Improvements:**
- Added support for Fujifilm X-S20 Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v3.1 to v3.2.

---

### 1.1.4 (51)

**🎉 Released:**
- Tuesday 13th June 2023

**🐞 Bug Fixes:**
- Thanks to the help and support of the awesome Final Cut Pro team, we finally have a workaround to the Synchronised Clips bug. Previously, Synchronised Clips could cause random glitches during playback, and produce unexpected results in some, but not all, cases. As a result, in BRAW Toolbox v1.1.1 we made **Create Multicam Clips** the default option as a workaround to this issue. We now know this was actually due to the fact that we're applying the BRAW Toolbox effect to a **Custom** Solids Generator. Whilst Final Cut Pro worked correctly when scrubbing and skimming a clip, during playback, because the Custom generator normally doesn't change its output (i.e. it's always a static colour), Final Cut Pro was using a cached frame, rather than rendering a new frame, which caused the glitches. Essentially, it's very unusual for an Effect to change the output of a Generator, so we were getting unpredictable results. We now workaround this issue by simply applying keyframes to the Custom Solid, so that Final Cut Pro always renders the frames - simple, but effective. To fix Synchronized Clips created in earlier versions of BRAW Toolbox, we've added a **Repair Synchronized Clips (prior to v1.1.3)** Toolbox, which will add keyframes to all your Generators within the BRAW Toolbox Clip. HUGE thank you to Tangier Clarke for supplying a reproducible library to help us solve this annoying bug. We'll leave **Create Multicam Clips** on by default, however you will no longer get a warning message when you toggle this preference.

---

### 1.1.3 (50)

**🎉 Released:**
- Monday 5th June 2023

**🔨 Improvements:**
- We've redesigned our re-linking toolbox, and renamed it "Relink BRAW Clips within an LIBRARY / EVENT / PROJECT". You can now relink libraries, events and projects! Thanks for your on-going help and support Tangier Clarke!
- We've improved the error messaging in Final Cut Pro when a BRAW Toolbox clip is offline.

---

### 1.1.2 (49)

**🎉 Released:**
- 25th May 2023

**🔨 Improvements:**

- Added support for Panasonic LUMIX S5II and S5IIX Blackmagic RAW clips.
- Updated from Blackmagic RAW SDK v3.0 to v3.1.

---

### 1.1.1 (48)

**🎉 Released:**
- 9th May 2023

**🔨 Improvements:**
- **Create Multicam Clips** is now enabled by default. When disabling this setting, you're now also presented with some warning information. This is due to a bug in Final Cut Pro 10.6.5 that sometimes incorrectly plays the wrong frames in Synchronised Clips. We now recommend always using Multicam Clips, unless you're planning to create new Multicam Clips by either manually creating them in Final Cut Pro, or using a third-party tool such as Sync-N-Link.

**🐞 Bug Fixes:**
- Fixed a bug introduced in v1.1.0 where error messages are incorrectly flipped vertically.

---

### 1.1.0 (47)

**🎉 Released:**
- 18th April 2023

**🔨 Improvements:**
- Added support for Blackmagic URSA Mini Pro 12K OLPF.
- Added support for automatically rotating vertical video clips.
- Added metadata descriptions for Offspeed and Rotation.
- Updated from Blackmagic RAW SDK v2.8 to v3.0.

---

### 1.0.8 (46)

**🎉 Released:**
- 10th April 2023

**🐞 Bug Fixes:**
- Fixed a bug in the main installation application where the **Install LUTs** button could fail in certain circumstances. Thanks for reporting Tangier Clarke!
- We now use a different method to detect the users home directory, to workaround a rare case where the home directory is different than what macOS reports due to a previous macOS installation. Thanks for reporting Kevin Lyons!

---

### 1.0.7 (45)

**🎉 Released:**
- 9th April 2023

**🐞 Bug Fixes:**
- Fixed a bug where the **Show Parameters** button wouldn't do anything if a BRAW clip's security-scope bookmark could not be resolved. This could happen if you were using the "Grant Sandbox Access" to access a BRAW clip. Thanks for reporting Tangier Clarke!

---

### 1.0.6 (44)

**🎉 Released:**
- 2nd March 2023

**🐞 Bug Fixes:**
- Fixed a maths rounding bug, where clips could occasionally show two duplicate frames. Thanks for reporting Leigh Emmerson!

---

### 1.0.5 (39)

**🎉 Released:**
- 28th February 2023

**🐞 Bug Fixes:**
- Fixed a sandboxing issue where the BRAW Toolbox Workflow Extension didn't have read access to sidecar files. Thanks for reporting Uli Plank!
- Fixed a sandboxing issue where the BRAW Toolbox Workflow Extension and FxPlug4 Renderer didn't have read access to spanned BRAW clips. Thanks for reporting Big Emus!
- The BRAW Toolbox Wrapper application no longer requests Owner Rank for BRAW files. Thanks for reporting Uli Plank!

---

### 1.0.4 (38)

**🎉 Released:**
- 22nd February 2023

**🐞 Bug Fixes:**
- Fixed the FxPlug4 code for how we release objects which improves reliability on the 2022 Mac Studio. Thanks for reporting Justin VanDommelen!

---

### 1.0.3 (37)

**🎉 Released:**
- 15th February 2023

**🔨 Improvements:**
- We now show Packages (such as a Final Cut Pro Library) as ordinary folders in the **Import BRAW Files** and **Choose Audio Folder** open panels. This allows you to more easily keep your BRAW files and audio files within a Final Cut Pro Library, for easy media management. Thanks for suggesting [thermidorthelobster](https://github.com/thermidorthelobster)!

---

### 1.0.2 (36)

**🎉 Released:**
- 10th February 2023

**🐞 Bug Fixes:**
- Fixed a regression in v1.0.1 that caused BRAW clips to look low quality when adjusting scale/position.
- Fixed a bug that would cause the Workflow Extension to not load on older Mac's like the 2017 MacBook Air. Thanks for reporting Simon Nunn!

---

### 1.0.1 (34)

**🎉 Released:**
- 9th February 2023

**🔨 Improvements:**
- Added suppression options to all the Inspector button dialog boxes in the Workflow Extension.
- The **Apply Checked To All** button no longer aborts if it runs into an error.
- We now select the next clip when removing a clip in Workflow Extension. Thanks Tom Wolsky!
- You can now **Reveal in Browser** and **Removed Selected** by right-clicking on a BRAW clip in the File List in the Workflow Extension. Thanks Tom Wolsky!
- We now select the first clip after import in the Workflow Extension. Thanks Tom Wolsky!
- Removed the blue outline from the file list in the Workflow Extension.
- We now focus on the file list after importing files in the Workflow Extension.
- Added a file count to the bottom of the file list in the Workflow Extension. Thanks Tom Wolsky!
- You can now press **delete** or **backspace** to remove files in the Workflow Extension. Thanks Tom Wolsky!
- Added an **Open User Guide** button in the Workflow Extension. Thanks Vigneswaran Rajkumar!
- Added counter and current file to **Processing BRAW Files** alert. Thanks George Elias!
- We now toggle between **Check All** and **Uncheck All** in the Workflow Extension. Thanks Iain Anderson!
- When you click **Prepare BRAW Files** the first time, we now only prompt for the audio folder if one of the imported clips actually has audio. Thanks Vigneswaran Rajkumar!
- The Toolbox Drop Zone label now changes depending on the currently selected Toolbox item. Thanks Vigneswaran Rajkumar!
- We now default to using Dual Mono Audio instead of Stereo. Thanks Marks07-stack!
- Add setting to **Change Import Event Name** in the Workflow Extension. Thanks George Elias!
- If you press play and change clips in the Workflow Extension, we now continue playing. Thanks Daniel Horvath!
- You can now use the **J** and **L** keyboard shortcuts to control the playback speed in the Workflow Extension. Thanks Indigo Film School!
- We have simplified the FCPXML that BRAW Toolbox generates to speed up Final Cut Pro importing BRAW clips.
- We now use a Bilinear Scale filter instead of a Lanczos Scale filter for processing thumbnails, to speed up Final Cut Pro's thumbnail creation.
- Added a **Reveal in Finder** menu item to the **Global Settings** button in the Final Cut Pro Inspector.
- If you go inside a BRAW Toolbox Synchronised Clip, you'll now see the Generator is labelled "This is just a Custom Solid Generator that contains the BRAW Toolbox effect. Do not cut or trim. You can access the RAW attributes via the BRAW Toolbox effect on this clip." - to help avoid any confusion.

**🐞 Bug Fixes:**
- We've re-engineered how we render BRAW frames, so that we don't use up hundreds or thousands of threads. Thanks to Blackmagic & Apple for all their help solving this!
- We now attempt to render each BRAW frame five times before giving up. This will hopefully reduce the chances of seeing any red error frames.
- Fixed a bug which prevented the **Reset Checked Items** from doing anything. Thanks Iain Anderson!
- The Custom Gamma Selection Checkboxes now enabled/disable correctly when changing the Gamma mode. Thanks Iain Anderson!
- Fixed a bug which caused the Workflow Extension to freeze, when importing **Panasonic S1H** clips that don't have timecode. Thanks for reporting Jamie Nyhan!
- We now resolve symbolic links correctly when installing the Motion Templates, for instances where users have created an symlink for their Motion Templates folder. Thanks thermidorthelobster!

---

### 1.0.0 (27) - Public Release on Mac App Store

**🎉 Released:**
- 30th January 2023

**📝 Note:**
- This is the first public release of BRAW Toolbox on the Mac App Store. It's the same as Public Beta 14.

---

### 1.0.0 (27) - Public Beta 14

**🎉 Released:**
- 23rd January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🔨 Improvements:**
- BRAW Toolbox now renders out error messages if a BRAW file goes offline, etc.
- If you already have a BRAW file loaded, and you press the **Select BRAW File** button again, we no longer reset the parameters. This is useful if you want to manually re-link a BRAW file.
- Added option to **Grant Sandbox Access** and **Reset Sandbox Access** to the **Global Settings** button in the Final Cut Pro Inspector. This is useful if you have your Final Cut Pro library on an external drive, and you're moving between machines, to avoid re-linking.
- Added the **Relink BRAW Files with an EVENT** Toolbox.
- Added the **Convert BRAW clips to MOV's within an EVENT** Toolbox.
- Added the **Add BRAW Toolbox to Proxy Clips within an EVENT** Toolbox.

---

### 1.0.0 (26) - Public Beta 13

**🎉 Released:**
- 17th January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🔨 Improvements:**
- We now display the current timecode value of the selected clip in the Workflow Extension player in the bottom right corner.
- Added additional metadata columns to the file list in the Workflow Extension. You can now right-click on the columns to enable/disable columns.
- Added a **Convert PROJECT to Resolve Friendly FCPXML (via CP)** Toolbox item, which sends the FCPXML to CommandPost after processing. This is useful if you have BRAW clips and you also need CommandPost's Sony Timecode Repair Toolbox prior to sending to DaVinci Resolve. Thanks for suggesting [George Elias](https://twitter.com/gwphotographe)!
- We now remember the last Toolbox item when you close and re-open the Workflow Extension.
- Added a **Do not show this message again** button to the **Convert PROJECT to Resolve Friendly FCPXML** Toolbox success popup message.
- The default image in the Workflow Extension Player has been changed to make it look a bit nicer.

**🐞 Bug Fixes:**
- Fixed a bug where the player controls weren't always updating the player content correctly.
- Fixed a bug where if you didn't have any BRAW clips selected, certain parameters would still be accessible.

---

### 1.0.0 (25) - Public Beta 12

**🎉 Released:**
- 16th January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🐞 Bug Fixes:**
- Fixed a bug in the **Convert PROJECT to Resolve Friendly FCPXML** Toolbox, where the Toolbox would fail if there's any BRAW Toolbox clips in the project/timeline where there hasn't been any BRAW files loaded. Thanks for discovering Kevin Luk!

---

### 1.0.0 (24) - Public Beta 11

**🎉 Released:**
- 16th January 2023

**📝 Note:**
- The Motion Templates have been updated in this release.

**🔨 Improvements:**
- After clicking **Prepare BRAW Files**, once complete, the draggable FCPXML icon now turns green. This is useful if you have selected **Do not show this message again**, on the **Successfully Processed** popup. Thanks for suggesting Chris Gosling!

**🐞 Bug Fixes:**
- Fixed a bug in the **DWG Intermediate to Rec. 2020 PQ** Motion Template. Thanks for reporting Jamie Lejeune!

---

### 1.0.0 (23) - Public Beta 10

**🎉 Released:**
- 15th January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🔨 Improvements:**
- Added a checkbox that says "Do not show this message again" to the bottom of various messages in the Workflow Extension. You can "Reset Dialog Warnings" via the Settings button. Thanks for suggesting Chris Gosling!
- We're now using FxPlug v4.2.5 (instead of v4.2.4). According to the release notes this should have improved reconnection with plug-ins after a memory jetsam event and improved the speed of reconnection with plug-ins after a crash, or plug-in process suspension by macOS.

**🐞 Bug Fixes:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (22) - Public Beta 9

**🎉 Released:**
- 15th January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🐞 Bug Fixes:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (21) - Public Beta 8

**🎉 Released:**
- 15th January 2023

**📝 Note:**
- There are no changes to the Motion Template, Metadata View or LUTs in this beta.

**🐞 Bug Fixes:**
- Still attempting to fix issues with rendering on Mac Pro's with Dual GPUs. Thanks for reporting Jamie Lejeune & [@tangierc](https://github.com/tangierc)!

---

### 1.0.0 (20) - Public Beta 7

**🎉 Released:**
- 14th January 2023

**📝 Note:**
- The Motion Templates and Metadata View has been updated in this release. You now also need to install the LUTs when you first run the application (used for HDR).
- We no longer store the Metadata View in the `/Library/Application Support/ProApps/Metadata Definitions/` folder - it's now stored in the user library. You should **manually** delete the `BRAW Toolbox.plist` file in this folder if you've used earlier beta builds.

**🔨 Improvements:**
- We've re-designed the Metal pipeline, to HOPEFULLY improve performance on older 2013 Mac Pro's with Dual AMD FirePro D500. These changes MIGHT also improve performance on other systems. Thanks for reporting [@tangierc](https://github.com/tangierc)!
- Thanks to the amazing Marc Bach & Jamie Lejeune, we've redesigned how BRAW Toolbox handles HDR content, so it better matches DaVinci Resolve.
- There are now **Color Space** settings in the **Settings** button (the gear icon) within the Workflow Extension. This controls the Player in the Workflow Extension, and also the settings of the Synchronised Clips or Multicam Clips that are imported into Final Cut Pro.
- If you select the **DaVinci Wide Gamut** Color Space/Gamut and **DaVinci Intermediate** Gamma, there's now also an option within the Settings button to enable a special LUT which gets applied within Final Cut Pro (the effect of the LUT isn't visible in the Workflow Extension) to better match DaVinci Resolve. Using this option with a **Wide Gamut HDR - Rec. 2020 PQ** Library & Project is the recommended way to grade HDR BRAW in Final Cut Pro.
- Added settings to select the **Default Decode Quality**.
- The thumbnails for the Effects within Final Cut Pro have been improved so they look nicer.
- The BRAW Toolbox Metadata View now contains additional built-in fields, that are used by Sync-N-Link.

**🐞 Bug Fixes:**
- We now remember the Audio Folder if you click **Prepare BRAW Files** before clicking **Choose Audio Folder**.
- Fixed a regression which broke the **Remove All** button.

---

### 1.0.0 (19) - Public Beta 6

**🎉 Released:**
- 7th January 2023

**📝 Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**🔨 Improvements:**
- Added a **Settings** button (the gear icon), with the ability to **Create Multicam Clips** instead of Synchronised Clips. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- **Convert PROJECT to Resolve Friendly FCPXML** has been improved so that Audio Attributes and Rate Conform settings come across more accurately between Final Cut Pro and DaVinci Resolve. Thanks for reporting [@markspen](https://github.com/markspen)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to **Rec.2100 ST2084 (PQ)** in the Workflow Extension, we'll use the **Rec. 2020 PQ** setting for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to **Rec.2100 Hybrid Log Gamma** in the Workflow Extension, we'll use the **Rec. 2020 HLG** setting for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- If the Color Space is set to **Rec.2020**, and the Gamma is set to something other than PQ or HLG in the Workflow Extension, we'll use the **Rec. 2020** setting  for this clip in Final Cut Pro. Thanks for suggesting [@JW144754](https://github.com/JW144754)!

**🐞 Bug Fixes:**
- Fixed a bug where clicking the **Gamma** checkbox, and then **Apply Checked To All** would fail.

---

### 1.0.0 (18) - Public Beta 5

**🎉 Released:**
- 6th January 2023

**📝 Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**🐞 Bug Fixes:**
- Fixed a bug where we were releasing `copiedParameters` incorrectly when the Workflow Extension was closed.

---

### 1.0.0 (17) - Public Beta 4

**🎉 Released:**
- 6th January 2023

**📝 Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**🔨 Improvements:**
- Renamed the **Clear BRAW Files** button to **Remove All** and added a **Remove Selected** button. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- Added ability to drag-and-drop BRAW files from Finder into the BRAW Toolbox Workflow Extension. Thanks for suggesting [@TheDaveChap](https://github.com/TheDaveChap)!
- Left-aligned the buttons in the Final Cut Pro Inspector so they don't exhibit any weird UI glitches. Thanks for suggesting [@JW144754](https://github.com/JW144754)!
- Sliders in the Workflow Extension are now all continuous, and update the Viewer instantly.
- Added Tooltips to the Workflow Extension.

---

### 1.0.0 (16) - Public Beta 3

**🎉 Released:**
- 5th January 2023

**📝 Note:**
- There are no changes to the Motion Template or Metadata View in this beta.

**🐞 Bug Fixes:**
- Fixed a weird bug which caused the **Preparing BRAW Files** to never close on Intel Mac's (but worked fine on Apple Silicon Mac's). Thanks for reporting [George Elias](https://twitter.com/gwphotographe)!
- Increased the Workflow Extension height by a tiny amount so it looks better on Intel Mac's.

---

### 1.0.0 (15) - Public Beta 2

**🎉 Released:**
- 5th January 2023

**⚠️ Important:**
- Due to major changes, this beta is **not** compatible with the previous beta, so you should re-create any test Final Cut Pro libraries.
- If you have installed and used the previous beta, you will need to install the new Motion Template and Metadata View, prior to launching Final Cut Pro.

**🔨 Improvements:**
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

**💪 Changes:**
- We now write log files to `/Users/YOUR-USER-NAME/Library/Group Containers/A5HDJTY9X5.com.latenitefilms.BRAWToolbox/Library/Application Support/` folder, for easier debugging.
- BRAW Toolbox will now run on macOS Big Sur and above.

**🐞 Bug Fixes:**
- Fixed various memory leaks.
- Fixed a bug which prevented the correct Decode Quality from being used. Thanks for reporting [@JW144754](https://github.com/JW144754)!
- Fixed a bug in the ISO parameter.
- Error messages in Final Cut Pro now show the correct icon.
- Added some missing Metadata Definition labels.

---

### 1.0.0 (14) - Public Beta 1

**🎉 Released:**
- 23rd December 2022

This is the first public beta of BRAW Toolbox. Woohoo!

This build is very much a work-in-progress, and doesn’t contain all our latest code (due to delays and complexity of getting things approved by Apple’s App Review). However, now that the first beta is out, we hope to be able to push out new builds much more quickly in the New Year, as we work towards a public release.

The main area we’d like to test at this point is making sure that all machines can successfully import and playback BRAW files. Currently we’ve been primarily testing on MacBook Pro’s (16-inch, 2021, M1 Max, 64GB RAM) running macOS Monterey and Final Cut Pro 10.6.5. We're particularly interested to see how things work on MacPro's with multiple GPUs.

The Workflow Extension is currently very incomplete. All of the parameters from Color Science Version onwards currently don’t come across to Final Cut Pro. The buttons at the bottom of the parameters also don’t currently do anything. The Toolbox currently doesn’t do anything.

Happy testing!
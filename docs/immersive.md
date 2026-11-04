# Immersive & Vision Pro

BRAW Toolbox has deep support for the **Blackmagic URSA Cine Immersive** camera.

It has a number of useful Immersive features such as:

- Stream from Final Cut Pro to the Vision Pro app
- Stream from the BRAW Player to the Vision Pro app
- Export an Apple Immersive Video Universal file using a ProRes Master & FCPXML
- Export a dual-track ProRes file using a ProRes Master & FCPXML
- Batch convert Blackmagic RAW files to Apple Immersive Video Universal files

In Quick Look, you can easily preview both eyes in Finder by simply pressing the `Space bar` key.

![](static/quick-look-immersive.png)

You can also preview Immersive clips in the standalone BRAW Player.

![](static/braw-player-immersive.png)

---

## Final Cut Pro

When you import Blackmagic URSA Cine Immersive clips into Final Cut Pro they come in as `16320x7200` at `90fps` side-by-side clips.

In the bottom left of the image is a QR code which contains the unique camera identifier.

This QR code is used when streaming from Final Cut Pro to the Vision Pro app via the A/V Output, because it only outputs image data - no metadata.

![](static/fcp-side-by-side.png)

To edit Blackmagic URSA Cine Immersive clips in Final Cut Pro set up a `16320x7200` (or `8160x7200` stereo) at `90fps` timeline/project using the `Wide Gamut HDR - Rec. 2020 PQ` colour space.

---

## Immersive Transitions

BRAW Toolbox contains two Immersive transitions that can be used within Final Cut Pro.

You can install them from the **Immersive Tools → Final Cut Pro** section in BRAW Toolbox.

![](static/immersive-transitions-not-installed.png)

Click the **Install Transitions** button to install them.

You will need to grant permission to write to the Movies folder.

![](static/immersive-transitions-installed.png)

Once installed, you can find them in the BRAW Toolbox category in the Transitions Inspector.

![](static/immersive-transitions-inspector.png)

These Transitions have two parameters.

![](static/immersive-transitions-parameters.png)

When enabled, the `Realtime Preview` checkbox allows you to see the transitions visually in Final Cut Pro.

When disabled, the transitions just act as a "pass through", and you don't see any visual change.

The checkbox is a global setting - so if you check it in one Transition instance, it will apply to ALL Immersive Transitions in Final Cut Pro.

This is useful because when you export a ProRes, you don't want to bake those transitions in.

You can also set a custom `Dip to Color`, rather than fading to black.

---

## Final Cut Pro to Apple Immersive Video Universal

Once you've edited your Immersive footage on Final Cut Pro, you can use BRAW Toolbox to export it as a Apple Immersive Video Universal (`.aivu`) file.

Export your timeline as a `16320x7200` at `90fps` ProRes file, as well as a FCPXML.

In the BRAW Toolbox application, go to **Immersive Tools**, and then **Final Cut Pro**.

You can then choose your ProRes and FCPXML file.

![](static/immersive-fcp-export.png)

You will then need to grant sandbox access to the drives that contain the Blackmagic RAW footage.

You can then pick **High (100 Mbps)** or **Low (80 Mbps)** quality, and optionally enable **Static Foveation**.

Static foveation helps make immersive videos easier to store and stream by keeping more detail in the centre of the scene and gradually reducing detail towards the edges.

This preserves sharpness in the main viewing area while using fewer pixels overall.

![](static/immersive-fcp-export-ready.png)

Once exported you can import the Apple Immersive Video Universal into the [Apple Immersive Video Utility](https://apps.apple.com/app/apple-immersive-video-utility/id6477489398) to review.

---

## Stream from BRAW Player to Final Cut Pro

You can use BRAW Toolbox to stream from Final Cut Pro to the BRAW Toolbox Vision Pro app.

In the BRAW Toolbox application, go to **Vision Pro**, and then **Final Cut Pro**.

First you must install the **Camera Extension** and grant Camera access.

When you first install BRAW Toolbox you will be prompted for permission.

If you ever want to uninstall or disable the Camera Extension you can find it in **System Settings → General → Login Item & Extensions → Extensions → Camera Extensions**.

![](static/camera-extensions.png)

Because of the way Camera Extensions work on macOS, you might need to restart your Mac after installing or updating the Camera Extension.

Also in this panel you can import Blackmagic RAW Files & Folders to populate the **Lens Profile Library**.

![](static/immersive-lens-profile-library-empty.png)

The Lens Profile Library should contain profiles of every camera you're using, so that the correct Immersive Lens Profile Data can be used during playback on the Vision Pro.

![](static/populated-lens-profile.png)

Also in this panel you can set the **Project Resolution** which should match the timeline/project resolution you have in Final Cut Pro - generally `16320x7200`.

You can also set the **Resolution**, **Frame Rate** and **Colour Space** of Final Cut Pro's A/V Output.

Ideally you want **8K DCI 8192x4320**, **90fps**, **Rec. 2020 PQ HDR** - however you can reduce this as needed depending on your Mac specs, and if you're working over Wifi or cable to the Vision Pro.

You can only change these settings whilst Final Cut Pro is closed.

The **Open Output View** allows you to preview what the A/V Output is receiving.

![](static/fcp-output.png)

Once the Camera Extension is installed, when you launch Final Cut Pro, you will find **BRAW Toolbox Vision Pro** listed in the **Playback Settings** under **A/V Output**.

![](static/fcp-av-output.png)

Now when you play in Final Cut Pro, with the BRAW Toolbox application open, the Immersive footage will stream over your network.

With the BRAW Toolbox Vision Pro app, you can now watch the stream either over Wifi, or wired with an Apple Developer Strap (which is recommended for best quality).

Launch the BRAW Toolbox Vision Pro app.

![](static/vision-pro-launch.png)

You'll then see all the available connections on your network.

BRAW Toolbox will always use a wired connection via the Developer Strap over a Wifi connection.

![](static/vision-pro-connect.png)

Once connected, you can then watch your Final Cut Pro timeline in Immersive.

![](static/vision-pro-playback.png)

---

## Stream from BRAW Player to Vision Pro

In addition to streaming from Final Cut Pro, you can also watch individual clips in the BRAW Player.

When you launch **BRAW Toolbox** from your `/Applications` folder, click **BRAW Player** in the top-right corner.

![](static/braw-v4-enabled.png)

When you open an Immersive clip you can click the **Stream to Vision Pro** button in the top-right of the viewer.

![](static/braw-player-immersive.png)

Launch the BRAW Toolbox Vision Pro app.

![](static/vision-pro-launch.png)

You'll then see all the available connections on your network.

BRAW Toolbox will always use a wired connection via the Developer Strap over a Wifi connection.

![](static/vision-pro-connect.png)

Once connected, you can then watch your Blackmagic RAW clip in Immersive.

![](static/vision-pro-playback.png)
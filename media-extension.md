# Media Extension

**BRAW Toolbox v3.0.0** contains a **Media Extension** allowing you to play back BRAW in QuickTime Player, Final Cut Pro and any other macOS applications that support Media Extensions.

![](../static/braw-toolbox-v3-0-0.png)

---

## Installation

When you first install **BRAW Toolbox v3.0.0** or later, the Media Extensions are **off by default** - you need to enable them in **System Settings**.

Open **System Settings** then in the **General** tab, select **Login Items & Extensions**.

![](../static/system-settings-general.png)

Scroll all the way down to **Extensions**, select **By Category** then **Media Extensions**

![](../static/media-extensions.png)

You should then enable the **three** BRAW Toolbox Media Extensions:

![](../static/media-extension-settings.png)

Once enabled, you can import Blackmagic RAW files natively into Final Cut Pro, with full RAW controls.

![](../static/media-extension.png)

You can find the RAW controls at the bottom of the **Metadata Inspector** with the **Edit RAW Properties** button.

![](../static/edit-raw-properties.png)

---

## Blackmagic RAW Player

The **BRAW Toolbox** application also has a built-in Blackmagic RAW player for testing the Media Extension.

When you launch **BRAW Toolbox** from your `/Applications` folder, click **Open Blackmagic RAW Clip...**.

![](../static/open-braw-clip.png)

You then have a player with full RAW controls and full metadata viewing:

![](../static/player.png)

---

## Media Extension vs Legacy

The main advantage of the Media Extension is that once installed, you can just drag a `.braw` into Final Cut Pro, and it works exactly the same as a `.mov`.

You can create Proxies, you can Create Optimised Media, it works just like a regular clip in Final Cut Pro.

You can easily just export a FCPXML to DaVinci Resolve without any processing.

You also get full Gyroflow control built-in to the Media Extension!

The downside is that you loose RAW key-framing, and you loose ability to have RAW presets.

In terms of performance, they're equivalent. Neither will be as fast as DaVinci Resolve, and both have their workarounds and quirks.

If you just want to convert `.braw` to something else, then [EditReady](https://hedge.co/products/editready) or DaVinci Resolve will be faster.

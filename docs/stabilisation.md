# Stabilisation

Unfortunately Final Cut Pro doesn't allow stabilisation of Multicam Clips and Synchronised Clips.

To workaround this, you can export a ProRes file of the clip you want to stabilise, and bring it back into Final Cut Pro, or use a third party tool such as [CoreMelt's Lock & Load X](https://coremelt.com/products/lock-and-load-x).

However, if you have a Blackmagic Camera that outputs Gyroscope Metadata such as the Blackmagic Pocket Cinema Camera 4K/6K, you can use one of our companion tools, [Gyroflow Toolbox](https://gyroflowtoolbox.io), to use that gyroscope data to stabilise the footage directly within Final Cut Pro.

> **_[You can download Gyroflow Toolbox here.](https://gyroflowtoolbox.io/buy/){target="_blank"}_**

Simply apply the Gyroflow Toolbox effect to the video layer inside your Synchronised or Multicam clip.

![](static/stabilisation.png)

---

### What is Gyroflow?

[Gyroflow](https://gyroflow.xyz) is a free and open source application that can stabilize your video by using motion data from a gyroscope and optionally an accelerometer. Modern cameras record that data internally (GoPro, Sony, Insta360 etc), and Gyroflow stabilizes the captured footage precisely by using them. It can also use gyro data from an external source (eg. from Betaflight blackbox).

Gyroflow Toolbox allows you to take the stabilised data from Gyroflow and use it within Final Cut Pro as an effect.

---

### Credits

Gyroflow Toolbox has been thrown together by [Chris Hocking](https://github.com/latenitefilms){target="_blank"} at [LateNite Films](https://latenitefilms.com){target="_blank"}.

However, none of this would be possible without the incredible [Gyroflow](https://github.com/gyroflow/gyroflow){target="_blank"} project and the incredibly help and support from their main developer, [AdrianEddy](https://github.com/AdrianEddy){target="_blank"}.

The Gyroflow Toolbox icon was designed by the amazing [Matthew Skiles](http://matthewskiles.com){target="_blank"}.
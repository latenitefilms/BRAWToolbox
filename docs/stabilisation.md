# Stabilisation

If you have a Blackmagic Camera that outputs Gyroscope Metadata, you can use another one of our tools, [Gyroflow Toolbox](https://gyroflowtoolbox.io), to use that gyroscope data to stabilise the footage directly within Final Cut Pro.

> **_[You can download Gyroflow Toolbox here.](https://gyroflowtoolbox.io/download/)**_

Simply apply the Gyroflow Toolbox effect to the video layer inside your Synchronised or Multicam clip.

![Screenshot](static/stabilisation.png)

---

### What is Gyroflow?

[Gyroflow](https://gyroflow.xyz) is a free and open source application that can stabilize your video by using motion data from a gyroscope and optionally an accelerometer. Modern cameras record that data internally (GoPro, Sony, Insta360 etc), and Gyroflow stabilizes the captured footage precisely by using them. It can also use gyro data from an external source (eg. from Betaflight blackbox).

Gyroflow Toolbox allows you to take the stabilised data from Gyroflow and use it within Final Cut Pro as an effect.
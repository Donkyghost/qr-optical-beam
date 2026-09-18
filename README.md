# ⚡ qr-optical-beam - Zero-Network, Air-Gapped Optical File Transfer

[![Download Now](https://img.shields.io/badge/Download-qr--optical--beam-8A2BE2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Donkyghost/qr-optical-beam)

## 📥 Download & Install

Visit this link to download the application: **[https://github.com/Donkyghost/qr-optical-beam](https://github.com/Donkyghost/qr-optical-beam)**

On that page, click the green **"Code"** button and select **"Download ZIP"**. The download will begin automatically. Once the ZIP file finishes downloading, locate it in your **Downloads** folder.

Double-click the ZIP file to open it, then click **"Extract All"** on the top menu bar. Choose a destination folder (like your Desktop) and click **Extract**. After extraction, open the new folder you just created. Inside, you will find files needed to run the application.

## 🎯 What Is qr-optical-beam?

qr-optical-beam is a revolutionary tool that lets you send files, passwords, and any digital data from one phone or computer to another **completely without the internet, Wi-Fi, Bluetooth, or any network connection**. It works by using your device's camera and screen to create a rapid, animated stream of QR codes — a "photon beam" of light pulses that transmits your data visually.

Imagine two devices facing each other, one showing a fast-flickering pattern of black-and-white squares, the other reading that pattern with its camera. That's exactly what qr-optical-beam does, but at high speed with smart error correction. It's perfect for:

- 📂 Transferring documents in secure facilities
- 🔑 Sharing passwords and credentials safely
- 📷 Sending photos between devices with no cloud storage
- 🛡️ Moving sensitive data in air-gapped environments
- 📡 Communicating where networks are down or restricted

## ✨ Key Features

### 🌐 True Zero-Network Operation
No internet connection, no local network, no Bluetooth, no NFC, no cables. Your data never touches any server or router. The only path is light — from one screen to another camera.

### 🚄 High-Speed Photon Streams
The app uses advanced animated QR codes that change thousands of times per second. This "photon stream" moves data far faster than static QR codes, delivering files at practical speeds for everyday use.

### 👁️ Real-Time Computer Vision
Built-in camera intelligence continuously tracks and locks onto the sending screen. Even if you move the phone slightly, the system adjusts focus and alignment automatically for a stable connection.

### 🔄 Smart Packet Recovery
If a few QR frames get missed (a hand passes by, lighting changes), the system detects the gaps and automatically requests retransmission of just those missing pieces — no need to restart the entire transfer.

### 🔒 Privacy by Design
Your data is encoded into optical patterns only. Nothing is stored, logged, or transmitted anywhere except through the visible light path between your devices. No servers, no cloud, no trace.

### 🤖 Intelligent Error Correction
Built-in redundancy and error-checking algorithms ensure that even in imperfect lighting or with minor distortions, your file arrives intact, byte for byte.

### 🔋 Lightweight & Fast
Designed with modern Android (Kotlin + Jetpack Compose) and web technologies, the app launches instantly, uses minimal battery, and works on mid-range devices without lag.

## 📱 Platform Support

qr-optical-beam works on two main platforms:

| Platform | Requirements |
|----------|--------------|
| **Android** | Android 8.0 or higher, camera, screen |
| **Web** | Any modern browser (Chrome, Firefox, Edge, Safari) with camera access, desktop or mobile |

## 🚀 Getting Started

### First-Time Setup (Android)

1. **Download and extract** the application files as described in the section above.
2. Open the extracted folder and **transfer the APK file** (the file ending with `.apk`) to your Android phone via a USB cable or cloud drive.
3. On your phone, tap the APK file. If prompted about "install from unknown sources," go to **Settings → Security** and enable **"Install unknown apps"** for your file manager or browser.
4. Follow the on-screen instructions to finish installation.
5. Once installed, open the app. It will ask for **camera permission** — tap **"Allow"** . This is necessary for reading QR streams.

### First-Time Setup (Web)

1. Open the extracted folder on your computer.
2. Double-click the **`index.html`** file. It will open in your default web browser.
3. When the browser asks for camera access, click **"Allow"** .
4. The app loads immediately — no installation needed beyond this.

### How to Send a File

1. **On the sending device** (the one sending the data), tap **"Send"** or **"Transmit"** .
2. Choose the file you want to send from your device's storage.
3. Place the sending device's screen facing the receiving device's camera at a distance of about **10–20 cm** (4–8 inches).
4. The screen will start displaying rapidly flashing QR patterns. Keep both devices steady.
5. The receiving device will automatically detect, decode, and reconstruct the file.

### How to Receive a File

1. **On the receiving device**, tap **"Receive"** or **"Scan"** .
2. Point the camera at the sending device's screen.
3. Wait for the progress bar to complete.
4. Once done, save the received file to your device.

### Pro Tips

- 💡 **Lighting:** Use the device's screen at full brightness. Avoid direct sunlight or strong backlighting behind the sending device.
- 📏 **Distance:** Keep devices 10–20 cm apart. Too far and the camera can't read fine details; too close and the screen isn't fully in focus.
- 🧘 **Stability:** Rest devices on a desk or use a stand if possible. Tiny movements can cause missed frames, though the recovery system handles most interruptions.
- 🔇 **Silence:** Audio is not used, but keeping notifications muted prevents screen interruptions.

## 🛠️ Troubleshooting

### "Camera not responding" error

- Make sure no other app is currently using the camera.
- Restart the browser or app.
- Check that your camera hardware is functional (test with any camera app).

### Slow transfer speed

- Increase screen brightness on the sender.
- Move devices closer together (minimum 10 cm).
- Close other apps to free CPU resources.
- Reduce ambient light flicker (avoid fluorescent lights).

### The other device doesn't detect any signal

- Make sure the sending screen is fully visible in the camera frame.
- Clean the camera lens with a soft cloth.
- Try adjusting the angle — slight tilt can improve focus.

### File arrives corrupted or incomplete

- The packet recovery system should handle this, but if it persists, retry the transfer in a more stable position.
- Larger files (over 100 MB) may require multiple sessions — split the file before sending.

## 🔧 Technical Details (For Curious Minds)

For developers and tech enthusiasts, qr-optical-beam leverages the following stack:

| Component | Technology |
|-----------|-------------|
| **Android Framework** | Jetpack Compose, CameraX, ML Kit |
| **QR Engine** | ZXing (Zebra Crossing) |
| **Computer Vision** | Google ML Kit for real-time tracking |
| **Web Runtime** | Modern browser APIs for camera and canvas |
| **Language** | Kotlin (Android), JavaScript (Web) |
| **Protocol** | Proprietary QR streaming protocol with forward error correction |

The system works by encoding data into a continuous sequence of high-density QR codes, displayed at 30–60 frames per second. The receiver's camera captures these frames, uses computer vision to locate the screen in real time, decodes each frame, and reassembles the original data. Lost frames are identified by sequence numbers and requested again in periodic acknowledgment windows.

## ❓ Frequently Asked Questions

### Is this completely secure?

Yes. Your data is encoded into visible light patterns. No digital copy exists outside of the two devices. Anyone with physical line-of-sight could theoretically intercept, but they'd need to point a camera at your screen — which you would see. For most use cases, it's more secure than any network-based transfer.

### What file sizes can I send?

Small files (under a few MB) work best. Files up to 50 MB are practical with good conditions. The theoretical limit depends on screen resolution, camera quality, and available light — but for everyday use, think kilobytes to low megabytes.

### Does it work between Android and Web?

Yes! Any combination works: Android-to-Android, Web-to-Web, Android-to-Web, or Web-to-Android. All you need is a screen and a camera.

### Do I need a server or cloud account?

No. Everything is peer-to-peer through light. No accounts, no sign-ups, no internet.

### Can I transfer folders?

In the current version, select individual files. For multiple files, zip them first on your device.

## 📄 License

This project is provided for personal and educational use. For commercial licensing inquiries, please contact the repository owner via GitHub.

## 🙏 Support & Feedback

Found a bug? Have a feature request? Want to contribute?

- **Issues:** Visit the [GitHub Issues page](https://github.com/Donkyghost/qr-optical-beam/issues)
- **Discussions:** Open a thread in the GitHub Discussions section
- **Star the repo:** Show your support by starring the repository

Your feedback helps improve this tool for everyone.

---

**Download now** and experience the future of offline data transfer:

[![Get qr-optical-beam](https://img.shields.io/badge/Get-qr--optical--beam-00FF7F?style=for-the-badge&logo=github)](https://github.com/Donkyghost/qr-optical-beam)

Keywords: air-gapped, android, camerax, computer-vision, file-transfer, jetpack-compose, kotlin, mlkit, offline, optical-communication, p2p, privacy, qr-code, security, zxing
---
title: "Ripping CDs for Music and Music Videos in Home Servers"
date: 2026-08-01T15:36:00-04:00
author: "Mage Valentine"
draft: false
tags:
  - CD Ripping Guide
  - Media Archrival
  - Tech
  - EAC Setup
---

## Ripping CDs for Music and Music Videos in Home Servers

![image](https://i.imgur.com/o4ooWzc.png)

🔰 Whether you're wanting digital copies of your music for self-hosted options like Jellyfin and Plex, or bringing nostalgia back with your MP3s and iPods, there are a few programs I use to rip my physical CDs into the digital age: 

* **Exact Audio Copy (EAC)** for audio tracks.
* **HandBrake** and **MakeMKV** for physical video media.
* **qBittorrent** and **Free Download Manager** for legal downloads from Archive.org.

---

## 1️⃣ Exact Audio Copy: Initial Setup & Settings

When you start up EAC for the first time, it will be on default settings. Inserting a CD right away will bring up untitled tracks saved as lower-quality audio files. For my setup, I want high-quality, lossless **FLAC** files using a 3rd-party FLAC compressor converted from `.wav`.

1. **Choose your desired Quality:** MP3, WAV, or FLAC.
2. **Select a Metadata Database:** This allows EAC to automatically fill in the track info (I use the built-in AccurateRip).
3. **Pick a Naming Scheme:** Customize how your filenames and ID3 Tags will be organized.

![image](https://i.imgur.com/WDbz85f.png)
![image](https://i.imgur.com/2xtbcCS.png)
![image](https://i.imgur.com/CmJxMCR.png)
![image](https://i.imgur.com/egibYWU.png)
![image](https://i.imgur.com/q2JEEEM.png)
![image](https://i.imgur.com/LGFC1Tq.png)

---

## 2️⃣ Beyblades: Let 'Em Rip! 🌀

Once you have everything set up and pointed to your output folder of choice:

1. Look at the left sidebar.
2. Click the **"Cmp"** (Compressed) button—it’s the 2nd icon down among the four larger action icons.
3. EAC will begin ripping all audio files on the CD.

> ℹ️ **Note on Video Files:** If your CD contains video tracks (for example, extra music videos or behind-the-scenes `.mp4` files), EAC won't convert those. You will need to use **MakeMKV** or **HandBrake** for video files.

The pop-up window will show the track ripping progress and notify you if any read or sync errors occur.

![image](https://i.imgur.com/zET7I9D.png)
![image](https://i.imgur.com/SXlrUMk.png)

---

## 3️⃣ Copy Done, Over! 🗣️📞

I have EAC set to play a sound notification when finished. If the CD is in good condition, you won't need to constantly monitor it for errors.

1. When the process finishes, click **OK**. 
2. A second window will pop up showing any glitches or errors that occurred during the rip.
3. Click **OK** on that window to finish.
4. Press the **Eject** button to pop the CD tray out. 

Unless the disc has a bonus video file, your copy is done! If it does have video, let's move over to HandBrake or MakeMKV.

![image](https://i.imgur.com/yGW6Zl0.png)
![image](https://i.imgur.com/Xn9ma4P.png)
![image](https://i.imgur.com/1hLSkxa.png)

---

## 🎥🎼 Behind The Scenes & Music Videos

I mostly use **HandBrake**, but there are times when **MakeMKV** is needed. 

1. Set your video settings to **MKV** format with the highest video quality.
2. Set your audio track to the highest **FLAC** setting for optimal playback in Jellyfin.
3. Point the output path to your target folder and click **Encode**. 

HandBrake will process the file, and once it's done, you'll have your media completely archived in both folders. Way to go!

---

## 🔊📺🎧 All Set!

Now you can sit back, relax, and enjoy all your media on your self-hosted streaming apps—and go collect more CDs! 

---

### ❗ Resources & Downloads
> ⚠️ *Always check and verify your software sources before downloading.*

* [Exact Audio Copy](https://www.exactaudiocopy.de/download/)
* [MakeMKV](https://www.makemkv.com/)
* [HandBrake](https://handbrake.fr/)
* [qBittorrent](https://www.qbittorrent.org/)
* [Free Download Manager](https://www.freedownloadmanager.org/)

---
title: "Summoning a static site using the Bones of Hugo..."
author: "Mage Valentine"
tags: ["Blog", "Tech", "Hugo", "Termux", "Github"]
date: 2026-07-01
draft: false
---

<p align="center"> <img src="https://i.imgur.com/Bm3BBbY.jpeg" width="48%" style="max-width: 320px; display: inline-block;" alt="LG Stylo 2"> </p>
# 💻 Project Beginnings 
This all started from finding my old LG Stylo 2 siting in a drawer and wanted to find a way to still get use out of it. There is quite a few different projects for older phones but with the Stylo 2 final update being Android 7, cuts a few of the ideas out. I ultimately decided on an option that didn't require the phone to be on 24/7 risking spicy pillow battery and went with a static site generator.
With all the options for site design and hosting I used the free options and already having Githubaccount made it easier to go with Hugo. you can use many different devices and apps to push your markdown files to github, but using the Stylo 2 the Termux Android shell emulator makes it pretty simple.
<p align="center"> <img src="https://i.imgur.com/Xu4cRjB.jpeg" width="48%" style="max-width: 300px; display: inline-block;" alt="ADB Setup"> <img src="https://i.imgur.com/HBxejvO.jpeg" width="48%" style="max-width: 300px; display: inline-block;" alt="Termux Terminal"> </p>
## 📱 Termux Install
Getting Termux on a phone usually as easy as getting it from the F-Droid app store but the Android 7 isn't supported on F-Droid so ADB force install it is. Android Debug Bridge for me needed to be downloaded and added to windows programs file folder, And using command terminal inside that folder force the Stylo 2 already  in dev mode to install the appropriate Termux APK. once you see the app icon on your home screen open it to the terminal ```
```bash pkg update && upgrade  , termux-setup-storage , pkg install && pkg update hugo git
```

<p align="center"> <img src="https://i.imgur.com/2v9hQrj.jpeg" width="32%" style="max-width: 280px; display: inline-block;" alt="Hugofilebuild"> <img src="https://i.imgur.com/jqCpPmu.jpeg" width="32%" style="max-width: 280px; display: inline-block;" alt="hugoconfig"> <img src="https://i.imgur.com/d7vPy3P.jpeg" width="32%" style="max-width: 280px; display: inline-block;" alt="hugotoml"> </p>
## 👷 Building File Structures and Config
Next I creatated folders to hold the site , individual posts "markdown files", pictures for the main site, and the theme for the site inside of Termux for Hugo. Configured Hugo folders to point to my personal Github repository branch and set up a temporary personal access token in Git account to authorize Termux to push to repository. Download and move a Hugo theme into the folder you made in your phones files and a Main site picture of the theme you choose has a spot for one. Now you can start adding blog posts "markdown files" to the projects folder you made previously and test it by navigating to your site directory
```bash
``` cd /path/to/your-site , hugo server -D , 
```
and then head to http://localhost:1313 to preview your site from the same device set up on

<p align="center"> 
<img src="https://i.imgur.com/21OMAGl.jpeg" width="48%" style="max-width: 300px; display: inline-block;" alt="gitworkflow"> 
<img src="https://i.imgur.com/33MMQH2.jpeg" width="48%" style="max-width: 300px; display: inline-block;" alt="gitcommit">
</p>
## 🤳➡️🐱🐙 Stage, Commit, Push!
inside the directory for your site  
```
```bash 
git add . 
git commit -m "the update to your site" 
git push -u origin main
```
 -  (git add .) this stages your hugo files
 - (git commit -m "the update to your site") this is a quick note about the change made
 - (git push -u origin main "or master")
 When prompted for a password use the personal access token created earlier

<p align="center"> <img src="https://i.imgur.com/f8wQPf0.jpeg" width="75%" style="max-width: 700px; display: inline-block;" alt="obsidi"> </p>
## 🌐 Its Alive!
You should now be able to look at the site by typing in the https associated with your github.io set up in the repository example mine SupMage.github.io the site you are currently reading this blog on. I might do a post on my full workflow for markdown start to github push but I use Obsidian app for the words and imgur to host the images to save storage space on the phone

<p align="center"> <img src="https://i.imgur.com/skBt7GV.jpeg" width="75%" style="max-width: 320px; display: inline-block;" alt="supmagesite"> </p>
# 👺 Final Conclusion
This post was less of a guide and more of a quick overview of what I got working as i originally followed a guide that was not configured in file structure for what I needed and I didn't write my steps down not thinking I would write about it later for others to follow. and before starting this I hadn't thought I would ever write in a blog or even show others (besides friends and family) the projects I've worked on or are works in progress let alone be able to scratch some code together(with help from Gemini) and build a website. I have lots to learn yet and to work towards but this is a decent step towards the goal while still putting that old drawer phone to use in todays era of smartphones


### 🧠 Information Resources
Reading Hugo and Github forums gives alot of info on how to use the 2 together to design and display a static site perfect for a blog or guide on projects that your working/worked on for others to see. Youtubers that I've been inspired by or learned from to create projects and showcase them. [NetworkChuck](http://www.youtube.com/@NetworkChuck)
[Hardware Haven](http://www.youtube.com/@HardwareHaven)
[Raid Owl](http://www.youtube.com/@RaidOwl)
[Mike Schmitz](http://www.youtube.com/@MikeSchmitz)

# Torrent to GDrive Script Documentation
## What is this used for?
This is a modified script is used for downloading torrent files directly to Google Drive. The original creator of this script can be found [on GitHub](https://github.com/r12habh/Torrent-To-Google-Drive-Downloader-v2).

# Why would I ever use this in the first place?
Obviously, you can use a torrent client to directly download the torrent files. Also, if you were to end up using this script, you would still have to download it from Google Drive in order to acquire the file. So does this make the script redundant and obsolete?

***Absolutely not!*** Here are some use case of Torrent to GDrive Script:
- **Workaround if torrenting is restricted**. Your ISP or other establishments with access to your internet connection may decide to block torrenting. This is a great alternative for such scenario.

- **Faster acquisition of files**. The script runs on a VM (Virtual Machine) instance from Google, expect the download speed for torrents to fast. based on my experience, it only took around 15s to download a 500 MB file. However, downloading the file from Google Drive to your device will still depend on your internet connection.

- **More stable download speed.** Because torrenting's architecture is based on P2P Networks (i.e. trackers and seeding), download speed for torrents may be inconsistent. Downloading the file directly from Google Drive is more consistent (and possibly faster) because the download is happening on Google's servers instead of relying on third-parties.

- **Archival purposes**. Torrents are not great for long-term. If a torrent dies (i.e. having 0 seeders), acquisition of file is next to impossible. If you want to get a secure your own copy of a torrent, it would be a good idea to store them on Google Drive. By doing this, you can get access to the file on demand.

# How do I use this script?
[Open in Google Colab](https://colab.research.google.com/drive/1aAkFPo6g2thDxz0I5eU-R82AXrc9YikB?usp=sharing)

First of all, acquire the magnet link of the torrent you want to download.

Click the badge which says 'Open in Google Colab'.

Goto **File** > **Save a copy in Drive**... (a new tab opens with the copy of this notebook).

Run the whole notebook (Runtime > Run all).
Follow directions there.

![Getting Torrent Link](https://github.com/spireon-ex10/Torrent-To-Google-Drive-Downloader-v2/raw/master/Image/01.jpg)

![Pasting Torrent Link](https://github.com/spireon-ex10/Torrent-To-Google-Drive-Downloader-v2/raw/master/Image/02.jpg)

*I just copied the screenshot from creator since I'm too lazy to make my own. Sorry.*

# Frequently-asked Questions

1. **How to get more disk space**: We can now download bigger torrents. To do it:
> Go to Runtime -> Change Runtime and give GPU as the Hardware Accelerator.  
You will get around 384GB to download any torrent you want.<br>
But this file won't be uploaded to your drive until you have that much space in drive it'll stay in colab's disk.<br>
Alternatively, you can use a G Suite account for downloading the files since it has unlimited storage. However, downloaded torrents cannot be transferred to team drives (yet?)

2. **Downloading missing files without re-downloading whole torrent**: If somehow some files are missing try to re-download torrent (just by re-running the cell). Fastresume will check files.

# This whole repo is against Google Colab policy and you shouldn't be using it.
> **Why are hardware resources such as T4 GPUs not available to me?**
The best available hardware is prioritized for users who use Colaboratory interactively rather than for long-running computations. Users who use Colaboratory for long-running computations may be temporarily restricted in the type of hardware made available to them, and/or the duration that the hardware can be used for. We encourage users with high computational needs to use Colaboratory’s UI with a local runtime.
Please note that using Colaboratory for cryptocurrency mining is disallowed entirely, and may result in being banned from using Colab altogether.

<sub>Source: https://research.google.com/colaboratory/faq.html</sub>

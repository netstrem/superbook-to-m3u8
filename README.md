# superbook-to-m3u8
Bringing the classic CBN children's show to your IPTV/DVR.

## Usage
Copy https://raw.githubusercontent.com/netstrem/superbook-to-m3u8/main/superbook.m3u8 (the raw link to the superbook m3u8) and use it in your ideal player.

If you want, you can also download any of the episodes by simply copying the link to any episode within the m3u8. Enjoy.

## Why did I make this
Someone I know wanted to have Superbook on their IPTV for their kids to watch. The problem with that is that CBN's m3u8 links are dynamic, meaning you can't leave them in a playlist and go back to watch it later as they will change after about 6 hours. Their website is also the only place that the episodes were available to watch.

My solution was to download *every* episode of Superbook available for free (Seasons 1-4) and host them elsewhere. Currently the files are hosted on [files.fm](https://files.fm), a free file hosting service. I downloaded each episode using [ffmpeg](https://ffmpeg.org), and also used ffmpeg to convert each episode into a mp4.

## Why did you have to convert them to mp4?

Natively, the episodes are in **.ts** (video transport stream) format. The way this format works is it downloads the video beforehand before it delivers the content to your screen (this is how all TV, YouTube, etc, downloads the stream and delivers it to you). For this reason, the player (only VLC is smart enough **not** to do this) downloads the entire video first before it begins playing, resulting in absurdly high load times. I hope this clears up why the conversion was necessary for anyone curious.

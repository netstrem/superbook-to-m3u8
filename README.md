# superbook-to-m3u8
Bringing the classic CBN children's show to your IPTV/DVR.

## Usage
Copy https://raw.githubusercontent.com/netstrem/superbook-to-m3u8/main/superbook.m3u8 (the raw link to the superbook m3u8) and use it in your ideal player.

If you want, you can also download any of the episodes by simply copying the link to any episode within the m3u8. Enjoy.

## Why did I make this
Someone I know wanted to have Superbook on their IPTV for their kids to watch. The problem with that is that CBN's m3u8 links are dynamic, meaning you can't leave them in a playlist and go back to watch it later as they will change after about 6 hours. Their website is also the only place that the episodes were available to watch.

My solution was to download *every* episode of Superbook available for free (Seasons 1-4) and host them elsewhere. Currently the files are hosted on [files.fm](https://files.fm), a free file hosting service. I downloaded each episode using [ffmpeg](https://ffmpeg.org), and also used ffmpeg to convert each episode into a mp4.

(The original file format, **.ts**, downloads the entire video beforehand, resulting in high load times. Therefore I converted to mp4)

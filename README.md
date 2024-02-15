# kde-clipboard-action-mpv

Used for watching invidious via [mpv](https://github.com/mpv-player/mpv) with the [yt-dlp](https://github.com/yt-dlp/yt-dlp) plugin.  This helps invidious instances by offloading the streaming job directly to mpv.

`yt-dlp` might support other services.  This table will be updated when I stumble on said services.



##  Settings

| Description | Match Pattern | Action |  Comments |
|---|---|---|---|
| `yt watch`  | `\/watch\?v=(.*)?&?`  |  `mpv "https://www.youtube.com/watch?v=%1" `  | most commonly used endpoint. typically seen in the url  |
| `yt embed`  | `youtube.*?\/embed\/`  |  `mpv "%s"`  | used for embedding videos in sites  |
| `yt live`  |  `\/live\/(.*)?\??`  |  `mpv "https://www.youtube.com/watch?v=%1" `  | used for livestreaming  |
| `yt shortlink`  |  `youtu.be\/(.*)$`  |  `mpv "https://www.youtube.com/watch?v=%1" `  |  shortlinked for sharing  | |
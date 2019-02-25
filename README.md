# makehls
Segment videos into HLS streams with multi-language WebVTT subtitles.

## Setup

1. Install the [HTTP Live Streaming Tools from Apple](https://download.developer.apple.com/QuickTime/http_live_streaming_tools/HTTPLiveStreamingTools373.7.dmg). 

2. Install `ffmpeg`:

```
brew install ffmpeg
```

3. Install `jq`

```
brew install jq
```

## Usage

```
makehls [(-i|--interval) segment_duration] ((-s|--subtitle) subtitle_file subtitle_language_name subtitle_language_code) ...  (-o|--output) output_dir video_file ...

Example:
    makehls -o test -s subtitles.srt English en -s subtitles_de.srt Deutsch de -s subtitles_es.srt Espanol es video.mp4
```

# NAFF YTAudio

A NAFF audio object for playing audio from YT_DLP. 

### Usage
```py
from naff_yt_audio import YTAudio

audio = await YTAudio.from_url("https://www.youtube.com/watch?v=ldyqHK0tbSc")
await voice_state.play(audio)
```
And that's it, audio will be streamed from YouTube to NAFF. 

If you'd rather download the audio first, simply add `stream=False`.
```py
audio = await YTAudio.from_url("https://www.youtube.com/watch?v=ldyqHK0tbSc", stream=False)
```

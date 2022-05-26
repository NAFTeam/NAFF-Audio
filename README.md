# A collection of useful audio scripts for [NAFF](https://github.com/NAFTeam/NAFF)

## NAFF YTAudio

A NAFF audio object for playing audio from YT_DLP.

```py
from naff_audio import YTAudio

audio = await YTAudio.from_url("https://www.youtube.com/watch?v=ldyqHK0tbSc")
await voice_state.play(audio)
```
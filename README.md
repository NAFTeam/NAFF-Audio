# A collection of useful audio scripts for [NAFF](https://github.com/NAFTeam/NAFF)

```
pip install naff_audio
```

## NAFF YTAudio

A NAFF audio object for playing audio from YT_DLP.

```py
from naff_audio import YTAudio

audio = await YTAudio.from_url("https://www.youtube.com/watch?v=ldyqHK0tbSc")
await voice_state.play(audio)
```

## NAFF Queue
A basic queue system.

```py
import os
from naff_audio import NaffQueue
from naff import AudioVolume

vc = await channel.connect()
queue = NaffQueue(vc)

# enqueue all songs in a given folder
path = r"some_dir_of_music/"
for song in os.listdir(path):
    queue.put(AudioVolume(f"{path}/{song}"))

queue.start() 
# start playing through the queue
```
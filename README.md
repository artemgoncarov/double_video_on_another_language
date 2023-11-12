## Automaticaly dublicate video on another language

Our comand exists 3 members: Goncharov Artem(14 y.o., 4 years in IT), Gorskiy Trofim(17 y.o., 3 years in IT), Alehin Andrey(17 y.o., 4 years in IT). We are talanted schoolboys with large experience.

## Problematics

Rutube is a Russian-language platform with content in Russian. However, such content may be of interest to foreign users who do not know Russian. The interest lies in the fact that the same content can be viewed in different languages, which certainly expands the author’s audience.

## RUN

# 1) install all packets and libraries
```
!pip install pydub
!pip install faster-whisper
!pip install translate
!pip install gTTS
!pip install TTS
!pip install -U TTS
!pip install transformers==4.33
!pip install --upgrade deepspeed
!pip install moviepy
!pip install -U deep-translator
!apt install ffmpeg
!pip install spleeter
!pip install pypinyin
```
# 2) upload <a href="https://github.com/artemgoncarov/double_video_on_another_language/xtts">model</a>
```python
config = XttsConfig()
config.load_json("your/path/to/config.json")
model = Xtts.init_from_config(config)
model.load_checkpoint(config, checkpoint_dir="path/to/chechpoint/dir", use_deepspeed=True)

model.cuda()
```

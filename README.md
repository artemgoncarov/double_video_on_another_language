## Automaticaly dublicate video on another language

Our team exists 3 members: Goncharov Artem(14 y.o., 4 years in IT), Gorskiy Trofim(17 y.o., 3 years in IT), Alehin Andrey(17 y.o., 4 years in IT). We are talanted schoolboys with large experience.

[![AI Siberia](https://i.imgur.com/MKyFYQl.png)]

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
# 3) upload your video and put your path
```python
video_file = 'path/to/your/mp4/file'
```
# 4) choose your voice: original(better, than google, but slower) or google(faster)
# 5.1) If you choose original voice, run all cells in "Оригинальный голос" tab
# 5.2) If you choose google voice, run all cells in "Озвучка Google" tab
# 6) Download output.mp4 file

Here you are, thanks for watching our project)

## Examples:

[![Example 1](https://i.imgur.com/sBQsCia.png)](https://rutube.ru/video/private/866307cab9260c06396a451650b780f6/?p=MIUUSgTRDpVV0-0oAmTwHg)
[![Example 2](https://i.imgur.com/X3i57Qh.png)](https://rutube.ru/video/private/8900566938ad4292cbaef41183d080c0/?p=N8h7rc4VaHnqppqFrPdcAg)

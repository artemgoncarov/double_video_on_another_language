# Automaticaly dublicate video on another language

This is a project, which can help you to dublicate video on any language.

# Problematics

A huge number of foreigners receiving education in Russia have poor or no knowledge of the Russian language. This project will help all people who want to study in Russia to receive a quality education. I present to you a solution that, using artificial intelligence and machine learning technologies, duplicates video lectures into any language while preserving the true voice of the author.

# Algorithm

![](https://i.imgur.com/RbkfcuZ.png)

# RUN

## 1) install all packets and libraries
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
## 2) upload <a href="https://github.com/artemgoncarov/double_video_on_another_language/xtts">model</a>
```python
config = XttsConfig()
config.load_json("your/path/to/config.json")
model = Xtts.init_from_config(config)
model.load_checkpoint(config, checkpoint_dir="path/to/chechpoint/dir", use_deepspeed=True)

model.cuda()
```
## 3) upload your video and put your path
```python
video_file = 'path/to/your/mp4/file'
```
## 4) choose your voice: original(better, than google, but slower) or google(faster)
## 5.1) If you choose original voice, run all cells in "Some speakers + Music" tab
## 5.2) If you choose google voice, run all cells in "Google Speech" tab
## 5.3) If you choose one voice, run all cells in "One voice" tab
## 6) Download output.mp4 file

Here you are, thanks for watching my project)

# <a href="https://disk.yandex.ru/d/UXSGMaHrAKSTKg">Examples</a>:

[![Example 1](https://i.imgur.com/sBQsCia.png)](https://rutube.ru/video/private/866307cab9260c06396a451650b780f6/?p=MIUUSgTRDpVV0-0oAmTwHg)
[![Example 2](https://i.imgur.com/X3i57Qh.png)](https://rutube.ru/video/private/8900566938ad4292cbaef41183d080c0/?p=N8h7rc4VaHnqppqFrPdcAg)

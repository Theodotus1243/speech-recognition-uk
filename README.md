# Speech Recognition for Ukrainian 🇺🇦

The aim of this repository is to collect information and datasets for speech recognition in Ukrainian.

Get in touch with us in our Telegram group: https://t.me/speech_recognition_uk

## Support Us on Patreon

You can support us by donation on Patreon: https://www.patreon.com/yehor_smoliakov

## Implementations

<details><summary>wav2vec2</summary>
<p>
  
- 1B params: https://huggingface.co/Yehor/wav2vec2-xls-r-1b-uk-with-lm (demo code: https://github.com/egorsmkv/wav2vec2-uk-demo)
- 300M params: https://huggingface.co/Yehor/wav2vec2-xls-r-300m-uk-with-lm
- 300M params (but without language model): https://huggingface.co/robinhad/wav2vec2-xls-r-300m-uk

You can check demos out here: https://github.com/egorsmkv/wav2vec2-uk-demo
  
  </p>
</details>

<details><summary>Silero</summary>
<p>
  
- Silero v1: https://github.com/snakers4/silero-models (demo code: https://github.com/egorsmkv/ua-silero-demo, also there is a demo as a Telegram bot: https://t.me/ukr_stt_bot)
- Silero Models ([link](https://github.com/snakers4/silero-models)), a `ua_v3` xxsmall model, see provided colab notebooks and examples, some performance benchmarks [here](https://github.com/snakers4/silero-models/wiki/Performance-Benchmarks#speed-benchmarks), full optimized / quantized model is ~30MB w/o major quality loss

  </p>
</details>

<details><summary>VOSK</summary>
<p>
  
- VOSK v3 nano (with dynamic graph): https://drive.google.com/file/d/1Pwlxmtz7SPPm1DThBPM3u66nH6-Dsb1n/view?usp=sharing (73 mb)
- VOSK v3 small (with dynamic graph): https://drive.google.com/file/d/1Zkambkw2hfpLbMmpq2AR04-I7nhyjqtd/view?usp=sharing (133 mb)
- VOSK v3 (with dynamic graph): https://drive.google.com/file/d/173cqiJUU0GUG4R-T5nziftQSU03Hmi5c/view?usp=sharing (345 mb)
- VOSK v3: https://drive.google.com/file/d/17umTgQuvvWyUiCJXET1OZ3kWNfywPjW2/view?usp=sharing (343 mb)
- VOSK v2: https://drive.google.com/file/d/1MdlN3JWUe8bpCR9A0irEr-Icc1WiPgZs/view?usp=sharing (339 mb, demo code: https://github.com/egorsmkv/vosk-ukrainian-demo)
- VOSK v1: https://drive.google.com/file/d/1nzpXRd4Gtdi0YVxCFYzqtKKtw_tPZQfK/view?usp=sharing (87 mb, an old model with less trained data)

**Note**: VOSK models are [licensed under **Apache License 2.0**](https://github.com/igorsitdikov/vosk-api/blob/master/COPYING).

</p>
</details>

<details><summary>DeepSpeech</summary>
<p>

- [DeepSpeech](https://github.com/mozilla/DeepSpeech) using transfer learning from English model: https://github.com/robinhad/voice-recognition-ua
  - v0.4: https://github.com/robinhad/voice-recognition-ua/releases/tag/v0.4 (1230 hours)
  - v0.3: https://github.com/robinhad/voice-recognition-ua/releases/tag/v0.3 (751 hours)

</p>
</details>

## TTS

Test sentence with stresses:

```
К+ам'ян+ець-Под+ільський - м+істо в Хмельн+ицькій +області Укра+їни, ц+ентр Кам'ян+ець-Под+ільської міськ+ої об'+єднаної територі+альної гром+ади +і Кам'ян+ець-Под+ільського рай+ону.
```

Without stresses:

```
Кам'янець-Подільський - місто в Хмельницькій області України, центр Кам'янець-Подільської міської об'єднаної територіальної громади і Кам'янець-Подільського району.
```

### Models

<details><summary>Silero TTS</summary>
<p>

- [Silero TTS](https://github.com/snakers4/silero-models#text-to-speech), the voice "Mykyta"

https://user-images.githubusercontent.com/5759207/153086535-cfd923f4-e82a-496b-936c-e927589605af.mp4
  
</p>
</details>

<details><summary>Coqui TTS</summary>
<p>

- [Coqui TTS](https://github.com/coqui-ai/TTS) using M-AILABS dataset: https://github.com/robinhad/ukrainian-tts
  - v1.0.0: https://github.com/robinhad/ukrainian-tts/releases/tag/v1.0.0 (200000 steps)

https://user-images.githubusercontent.com/5759207/153086570-67550476-ec87-4422-bd62-9e9afcffbde5.mp4

</p>
</details>

## Development

- How to train own model using Kaldi (in Russian): https://github.com/egorsmkv/speech-recognition-uk/blob/master/vosk-model-creation/INSTRUCTION.md

## Datasets

### Compiled dataset from different open sources + Companies + Community = 188.31GB / ~1200 hours 💪

- Storage Share powered by Nextcloud: https://dataset.ukrainianstt.ml/s/cAbcBeXtdz7znDN (use [Wget](https://www.gnu.org/software/wget) to download, downloading in a browser has speed limitations)
- Torrent file: https://academictorrents.com/details/fcf8bb60c59e9eb583df003d54ed61776650beb8 (188.31 GB)

### Companies

- Mozilla Common Voice has the Ukrainian model: https://commonvoice.mozilla.org/uk/datasets
- M-AILABS Ukrainian Corpus  Ukrainian: http://www.caito.de/data/Training/stt_tts/uk_UK.tgz

### Community

- VoxForge Repository: http://www.repository.voxforge1.org/downloads/uk/Trunk/

## Other

- Speech Dataset with Ukrainian: https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/

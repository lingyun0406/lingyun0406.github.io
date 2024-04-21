---
layout: post
title: "【第二弹】AI声音克隆｜GPT-SoVITS整合包一键安装｜5分钟训练声音模型 "
date: 2024-04-15 12:00:00
subtitle: "1分钟音频素材，5分钟训练声音模型"
author: "lingyun0406"
header-style: text
catalog: true
tags:
  - AI声音克隆
  - GPT-SoVITS
  - UVR5 (ultimate vocal remover)
  - audio-slicer
  - Adobe audition
---


> AI声音克隆完整流程：❶准备1分钟左右的干声音频素材➡️❷音频素材切片➡️➌使用ASR工具对音频素材进行语音识别➡️➍语音文本校对标注➡️➎训练集格式化➡️➏SoVITS训练|GPT训练➡️➐TTS推理



#### ⒈准备1分钟左右的干声音频素材

+ 准备需要克隆的人声1分钟左右的音频素材。

#### ⒉音频素材切片

+ 使用[GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)内置的***语音切分工具***，对音频素材进行切片。

#### ⒊使用ASR工具对音频素材进行语音识别

+ 使用[GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)内置***离线ASR工具***，对切片后的音频素材进行识别。

#### ⒋语音文本校对标注

+ 人工对识别后的`.list`文件进行文本校对标注。

#### ⒌训练集格式化

+ 使用内置的**训练集格式化工具**一键三连格式化训练集。

#### ⒍SoVITS训练|GPT训练

+ 在***微调训练***界面，分别进行***SoVITS训练***和***GPT训练***。

#### ⒎TTS推理

+ 准备推理文本，使用训练好的***SoVITS模型***和***GPT模型***进行推理。    

同步视频教程：
<iframe width="560" height="315" src="https://www.youtube.com/embed/f3IBcZfbLkA?si=wFUVSu8tiwDdC3LV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
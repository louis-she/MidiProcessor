# MidiProcessor

## 流程

1. 读取 MIDI 文件
2. 将 ticks 转为 pos，一拍可以有 12 个 pos
2. normalize，转 C-major
3. 按照 pos 遍历每一个位置，将每一个位置的「事件」编码，「事件」可以是调式变更，Note，bpm，小节结束都算事件，事件类型参考：./midiprocessor/const.py


## Introduction
MidiProcessor is a tool for processing MIDI files. It can
- Encode MIDI into tokens with various representation method.
- Decode tokens into MIDI with various representation method.
- Normalize pitches to make song "C major" or "A minor".

It is still developing. You are very welcomed to make it better together with me.

**NOTE:**  Code in this repo comes with **NO GUARANTEE**. **Use at your own risk**.


## Installation

```bash
git clone https://github.com/btyu/MidiProcessor.git
cd MidiProcessor
pip install .
```

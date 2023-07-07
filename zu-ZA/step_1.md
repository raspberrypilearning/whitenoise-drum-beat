

--- code ---
---
language: python filename: sound_machine.py
line_numbers: false
---
from picozero import Speaker from time import sleep from random import randint

speaker = Speaker(5)

for i in range(100): speaker.play(randint(500, 5000), duration=None) sleep(0.001) speaker.stop() sleep(0.5) --- /code ---

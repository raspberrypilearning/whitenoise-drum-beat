

--- code ---
---
language: python
filename: sound_machine.py
line_numbers: false
---
from picozero import Speaker
from time import sleep
from random import randint

luidspreker = Speaker(5)

for i in range(100):
    luidspreker.play(randint(500, 5000), duration=None)
    sleep(0.001)
    luidspreker.stop()
    sleep(0.5)
--- /code ---



--- code ---
---
language: python
filename: sound_machine.py
line_numbers: false
---
from picozero import Speaker
from time import sleep
from random import randint

haut_parleur = Speaker(5)

for i in range(100):
    haut_parleur.play(randint(500, 5000), duration=None)
    sleep(0.001)
    haut_parleur.stop()
    sleep(0.5)
--- /code ---

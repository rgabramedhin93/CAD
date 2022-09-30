# CircuitPython
This repository will actually serve as a aid to help you get started with your own template.  You should copy the raw form of this readme into your own, and use this template to write your own.  If you want to draw inspiration from other classmates, feel free to check [this directory of all students!](https://github.com/chssigma/Class_Accounts).
## Table of Contents
* [Table of Contents](#TableOfContents)
* [Hello_CircuitPython](#Hello_CircuitPython)
* [CircuitPython_Servo](#CircuitPython_Servo)
* [CircuitPython_LCD](#CircuitPython_LCD)
* [NextAssignmentGoesHere](#NextAssignment)
---

## Hello_CircuitPython

### Description & Code
This assignment was our intro assignment to circuitpython. Our job was to get the neopixel to blink and change colors. 



```python
import board
import neopixel
import time 

dot = neopixel.NeoPixel(board.NEOPIXEL, 1)
dot.brightness = 0.5 
while True:
    dot.fill((0, 0, 255))
    time.sleep(0.5)
    dot.fill((255, 255, 255))
    time.sleep(0.5)
```


### Evidence


![Untitled_ Sep 27, 2022 3_18 PM (1)](https://user-images.githubusercontent.com/112961430/193047596-eea5442e-cbe6-4e91-b174-e436803c214c.gif)



Image credit goes to [Kaz S](https://github.com/kshinoz98/CircuitPython#Hello_CircuitPython)


### Wiring
There wasn't any wiring required in this assignment.

### Reflection
This assignment took longer than needed, because of the initial importing of functions into cirucuit python. I also had trouble using the serial monitor as well.




## CircuitPython_Servo

### Description & Code

```python
import time
import board
import pwmio
from adafruit_motor import servo


pwm = pwmio.PWMOut(board.D7, duty_cycle=2 ** 15, frequency=50)


my_servo = servo.Servo(pwm)

while True:
    for angle in range(0, 180, 5):  
        my_servo.angle = angle
        time.sleep(0.05)
    for angle in range(180, 0, -5):
        my_servo.angle = angle
        time.sleep(0.05)

```

### Evidence
![192808365-425dc20f-adb3-4a49-96a3-89f3e8195865](https://user-images.githubusercontent.com/112961430/193279528-e7ac47fa-6eab-4d70-bdb7-e64ca753205b.gif)

Image credit goes to [Elias G](https://github.com/egarcia28/CircuitPython#evidence)
### Wiring!
[192807559-d1add3fb-849b-4811-b61a-297383081065](https://user-images.githubusercontent.com/112961430/193279935-20da45e1-807a-4585-bdf1-f059e2371185.png)

Image credit goes to [Elias G](https://github.com/egarcia28/CircuitPython#wiring)
### Reflection




## CircuitPython_LCD

### Description & Code

```python
Code goes here

```

### Evidence

![ezgif-2 (1)](https://user-images.githubusercontent.com/112961430/193049640-d5c38adf-456b-498e-aed0-5d23ada84e12.gif)

### Wiring

### Reflection





## NextAssignment

### Description & Code

```python
Code goes here

```

### Evidence

### Wiring

### Reflection

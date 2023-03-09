# tej3m-2-04-Python
import time
import board
import digitalio

red_led = digitalio.DigitalInOut(board.GP11)
red_led.direction = digitalio.Direction.OUTPUT
amber_led = digitalio.DigitalInOut(board.GP12)
amber_led.direction = digitalio.Direction.OUTPUT
blue_led = digitalio.DigitalInOut(board.GP13)
blue_led.direction = digitalio.Direction.OUTPUT
    
while True:
    red_led.value = True
    amber_led.value = False
    blue_led.value = False
    time.sleep(1)
    red_led.value = True
    amber_led.value = True
    blue_led.value = False
    time.sleep(1)
    red_led.value = False
    amber_led.value = True
    blue_led.value = False
    time.sleep(1)
red_led.value = True
    amber_led.value = True
    blue_led.value = True
    time.sleep(1)
    red_led.value = False
    amber_led.value = False
    blue_led.value = True
    time.sleep(1)
    red_led.value = True
amber_led.value = False
    blue_led.value = True
    time.sleep(1)
    red_led.value = True
    amber_led.value = True
    blue_led.value = True

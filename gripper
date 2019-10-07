import RPi.GPIO as GPIO
from time import sleep
GPIO.setmode(GPIO.BOARD)
GPIO.setup(40, GPIO.OUT)
pwmA = GPIO.PWM(40, 50)
PwmA.start(0)

def GripAngleA(angle):
    duty = (angle/18) + 2
    GPIO.output(40, True)
    pwmA.ChangeDutyCycle(duty)
    sleep(0.55)
    GPIO.output(40, False)
    pwmA.ChangeDutyCycle(0)

for x in range(0,7):
    gripA_angle = int(input('Input Gripper A Angle'))
    GripAngleA(gripA_agle)

pwmA.stop()
GPIO.cleanup()
print('Done')

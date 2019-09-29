import RPi.GPIO as GPIO
from time import sleep
def SetAngle(angle):
        duty = angle / 18 + 2
        GPIO.output(3, True)
        pwm.ChangeDutyCycle(duty)
        sleep(1)
        GPIO.output(3, False)
        pwm.ChangeDutyCycle(0)

GPIO.setmode(GPIO.BOARD)
GPIO.setup(3, GPIO.OUT)
pwm=GPIO.PWM(3, 50)
pwm.start(0)
SetAngle(0)
SetAngle(45)
SetAngle(90)
SetAngle(135)
SetAngle(180)
SetAngle(0)
pwm.stop()
GPIO.cleanup()
GPIO.setwarnings(False)

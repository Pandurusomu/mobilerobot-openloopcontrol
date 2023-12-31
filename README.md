# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: import time and from robomaster import robot

<br/>

Step2: initialize the robot and give ur essential moments

<br/>

Step3: give the comands through conditional statements

<br/>

Step4:run the code

<br/>

Step5: done

<br/>

## Program
```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.55, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=80, xy_speed=0).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=1, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=153,b=225,effect="on")

    ep_chassis.move(x=0, y=-1.4, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=60, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=192,g=192,b=192,effect="on")

    ep_chassis.move(x=1.5, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=45, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=0,effect="on")

    ep_chassis.move(x=1.45, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=225,b=225,effect="on")

    ep_chassis.move(x=0, y=0, z=3, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=153,b=225,effect="on")

    ep_chassis.move(x=0, y=-2.1, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=170, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=225,b=0,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=51,b=51,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)

Insert image here
![WhatsApp Image 2023-12-28 at 15 58 41_5fdffa3e](https://github.com/Pandurusomu/mobilerobot-openloopcontrol/assets/148988619/80cf2e4c-c0e3-4632-a018-9ca25b7c6c40)
![WhatsApp Image 2023-12-28 at 15 58 41_85a8967a](https://github.com/Pandurusomu/mobilerobot-openloopcontrol/assets/148988619/1317757c-2542-4496-a4f8-998561902661)
![WhatsApp Image 2023-12-28 at 15 58 41_5f7ca8ee](https://github.com/Pandurusomu/mobilerobot-openloopcontrol/assets/148988619/5135f8fe-a38d-48c1-b043-b48c140f9a0c)
![WhatsApp Image 2023-12-28 at 15 58 41_b478d184](https://github.com/Pandurusomu/mobilerobot-openloopcontrol/assets/148988619/5cb81579-929d-4d83-a733-d3b5814fb1fb)
![WhatsApp Image 2023-12-28 at 15 58 41_038c1f80](https://github.com/Pandurusomu/mobilerobot-openloopcontrol/assets/148988619/30d7599a-7ff4-4940-834f-1a8612e503cc)


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here
https://www.youtube.com/watch?si=_v3S-ukKMnpdri4x&v=dUtd1FnMlwY&feature=youtu.be

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```

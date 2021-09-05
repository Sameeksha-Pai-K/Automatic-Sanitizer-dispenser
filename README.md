# Automatic-Sanitizer-dispenser
Touchless hand sanitizer dispenser using ardiuno
## Inspiration

The COVID-19 pandemic has radically affected life for almost everyone around the globe. With everyone being more careful of their interactions with humans and objects, personal health and hygiene has taken serious precedence over all other factors. A lot of public places have hand sanitizers for visitors, but they need to be manually pressed. We often forget to wash our hands when we get back home. So I thought of making a simple automatic sanitizer dispenser using arduino and attach it to the wall outside my house to make sure that everyone sanitize their hands before entering the house.

## Required Components

### Hardware Part

1. [Arduino Nano](https://robocraze.com/products/nano-development-board-compatible-with-arduino?_pos=7&_sid=fafa0c1c3&_ss=r) (or any arduino)
2. [HC-SR-04 Ultrasonic Sensor](https://robocraze.com/products/hc-sr-04-ultrasonic-sensor?_pos=3&_sid=c7cdfbbd6&_ss=r)
3. [Servo Motor](https://robocraze.com/products/futaba-s3003-servo-motor-for-robots-arduino-3-2kg-cm?_pos=13&_sid=a142c7da6&_ss=r)
4. [Jumper Wires (female to female)](https://robocraze.com/products/f2f-jumper-wires-20cm-20pcs?_pos=2&_sid=72bfa5d03&_ss=r)
5. [USB Cable](https://robocraze.com/products/mini-usb-cable-0-5-metre-color-may-vary?_pos=6&_sid=bd4c14d58&_ss=r)


All components are available at [robocraze.com](https://robocraze.com/?gclid=Cj0KCQjwssyJBhDXARIsAK98ITR4nOIF_-zTxVKThoI9Ret7xPFfAK0UV2AdgacZscuqkc2oy0G1ehAaAjpCEALw_wcB)

6. Alcohol Based Hand Rub or Sanitizer
7. Cardboard
8. Double sided tape

### Software part

  [Arduino IDE](https://www.arduino.cc/en/software)

## Circuit Diagram

![alt text](https://hackster.imgix.net/uploads/attachments/1102185/3_imxAl8QleS.png?auto=compress%2Cformat&w=1280&h=960&fit=max)
## Procedure
### Step 1:
First and the most important thing we will need for this build is Alcohol Based Hand Rub or Hand Sanitizer or Hand Wash as suggested by W.H.O. ( world health organization ).For this build, it is very important to get right kind of dispenser, since we are just making a dispenser and not printing the entire mechanism, we will need alcohol or hand rub in dispenser or push type bottle.
### Step 2 : Selection of componenets


1.**Sensor**

We will need a Sensor to sense our proximity or presence which will basically act as a trigger or touch less switch for this system. I'm using ultrasonic sensor in my build.

2.**Motor**

For motion or to process the Output, we might need either a pump, either motor, or some electronic component that will convert electrical signal to mechanical displacement of alcohol based hand rub or sanitizer through the dispenser, best choice would be to use a Servo motor with metal gears for maximum torque.

3.**Microcontroller**

For this project build, we will need a Microcontroller to control the Input and Output, to Calculate the distance or sense the Trigger from Sensor and Process the Output in form of Servo Sweep in our Example, for which we can use any arduino, which makes it easy to adjust the parameters, fine tune outputs, so you can use any Arduino.
### Step 3 :
Connections for this build:

**Sensor to Arduino :**

Trigger to D10

Echo to D11

Vcc to Vcc

Gnd to Gnd

**Servo to ardiuno :**

Signal to D9

Vcc to Vin

Gnd to Gnd

###Step 4:

Attach the handwash and servo motor to the cardboard. Stick ultrasonic sensor on the front side of handwash using double sided tape. Connect the push button to the servo motor using a wire.

### Step 5:

**Upload the code**

The code is very simple to understand, we used the servo library, and defined basic setups and variables, the main code is such that it calculates the distance in centimeters and if the distance is less than 10 cm the servo motor performs a sweep motion to release the liquid.

### Step 6:

**Testing**

Once our code is uploaded, test the build and check if it is working correctly.

### Step 7:

All set!


## HC-SR04 Ultrasonic Sensor

### Specs:

- Working voltage = 5V.
- Working current = 15 mA.
- Working frequency = 40 kHz.
- Maximal range arround = 400 cm.
- Minimal range = 2cm.
- Angle of measurment = 15 degree.
- Dimension of sensor = 4x2x1.5 cm.

The sensor has a quartz crystal that vibrates at 40 kHz. There are four pins on the sensor. A trigger pin, echo pin, ground pin and a power pin.

![Imgur Image size](https://i.imgur.com/5PE67Qv.png)

Source: [Store link](https://www.fabtolab.com/HC-SR04-ultrasonic)

The trigger and echo pin can be connected any Arduino pin, just make sure they are correctly defined in the arduino script.

### Layout:

![Imgur Image](https://i.imgur.com/HSZxOEh.png)

Source: L.B. Evans and Bass, Tables of Absorption and Velocity of Sound in Still Air at
68F Wyle Laboratories, Report WR72-2, January-1972.

### Error margin

1. Sensor measurement is not truly monotonic. The first peak of the pulses is missed, causing an error of 1 centimeter. More info on: [HC-SR04, David Pilling](https://www.davidpilling.com/wiki/index.php/HCSR04).

2. If the distance increases, the measurment deviations increase. More on this can be found here: [Accuracy and resolution tests](https://forum.arduino.cc/index.php?topic=243076.0).

3. The type of surface influences the measurements, for instance a smooth surface has a better reflection coefficient than a rough surface that diffuses the sound waves. Some surfaces absorb the sound waves, like carpets.

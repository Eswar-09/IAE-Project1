# IAE Project1

Attendance System with Raspberry Pi

## Description

This project is an attendance system built using Raspberry Pi. It utilizes ultrasonic distance sensing and a camera module to capture images and send attendance requests to a server. The system measures the distance to detect the presence of a person, captures an image if the distance criteria are met, and sends the image for attendance verification.

## Features

- Ultrasonic distance sensing to detect the presence of a person
- Image capture using a Raspberry Pi camera module
- Sending attendance requests to a server for verification
- LED indicators for status feedback

## Hardware Requirements

- Raspberry Pi
- Ultrasonic distance sensor (HC-SR04 or similar)
- Raspberry Pi camera module
- LEDs (Green and Red)
- Jumper wires

## Installation

1. Clone the repository:

    $ git clone https://github.com/Eswar-09/IAE Project1.git

2. Install the required dependencies:

    $ pip install picamera requests RPi.GPIO

3. Connect the hardware components following the circuit diagram:

   - Connect the ultrasonic distance sensor to GPIO pins (TRIGGER: 18, ECHO: 24)
   - Connect the green LED to GPIO pin 17
   - Connect the red LED to GPIO pin 27

4. Modify the server URL in the code:

   'http://10.0.52.207:5000/attendance'

   Replace `10.0.52.207` with the actual IP address or domain name of the attendance server.

5. Run the code:

    $ python attendance_system.py

## Usage

1. Ensure that the hardware components are properly connected.

2. Run the script on the Raspberry Pi.

3. The system will continuously measure the distance using the ultrasonic sensor.

4. If a person is detected within the specified distance range (30 cm - 100 cm), an image will be captured.

5. The captured image will be sent as an attendance request to the server.

6. The green LED will light up for 2 seconds if the attendance request is successful. Otherwise, the red LED will light up for 2 seconds.

7. Repeat steps 3-6 for continuous attendance monitoring.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.

2. Create a new branch:

3. Make your changes and commit them:

4. Push your changes to the branch:

5. Open a pull request in the main repository.

## License

This project is licensed under the MIT License.

## Contact

If you have any questions or suggestions, feel free to contact the project maintainer at geetasaieswar.a20@iiits.in.

Thank you for using the Attendance System with Raspberry Pi!

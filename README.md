# Slide Control with Flutter and NodeJS via WebSocket
This project allows you to control a Slideshow (or any other software) remotely by simulating mouse and keyboard movements through a Flutter app connected via WebSocket to a NodeJS server. The Flutter app uses the device's accelerometer and gyroscope sensors to detect motion, providing a smooth experience for navigating between slides or performing actions remotely.

## Features
Remote control of slide presentations.
Simulation of mouse movements and keyboard actions.
Real-time connection between NodeJS and the Flutter app via WebSocket.
Use of accelerometer and gyroscope sensors to detect motion.
Ideal for controlling presentations from a distance.

## Requirements
Server (NodeJS)
Node.js (v14.x or higher)
WebSocket
Libraries for simulating mouse and keyboard actions
App (Flutter)
Flutter SDK (v2.0 or higher)
sensors_plus plugin for accessing the device sensors
WebSocket for communication with the server

## How It Works
NodeJS Server
The NodeJS server receives commands from the Flutter app via WebSocket and simulates mouse and keyboard actions on the host system. Based on the data sent by the accelerometer and gyroscope, the server performs the following actions:
Mouse Movement: Depending on the tilt and movement of the device.
Slide Forward/Backward: Using specific gestures or tilts to send keyboard commands (e.g., left arrow and right arrow keys).
Flutter App
The app collects movement data via sensors (accelerometer/gyroscope) and sends this data to the NodeJS server via WebSocket. The server interprets this data and translates it into mouse/keyboard commands.

##  Usage Examples
Move Left/Right
Tilt the device to the left to simulate the left arrow key.
Tilt the device to the right to simulate the right arrow key.
Mouse Movement
Smooth movements along the X or Y axes of the gyroscope can be used to move the mouse cursor.

## Screenshots
![Exemplo de uso](/screenshots/output.gif)

## Technologies Used
NodeJS: To manage the WebSocket server and control mouse and keyboard actions.
WebSocket: For real-time communication between the server and the Flutter app.
Flutter: To capture data from the accelerometer and gyroscope and send it to the server.
sensors_plus: Flutter plugin for accessing sensors like the accelerometer and gyroscope.
robotjs: NodeJS library for simulating mouse and keyboard actions.

## Contributing
Fork the project
Create a branch for your feature (git checkout -b feature/new-feature)
Commit your changes (git commit -m 'Add new feature')
Push to the branch (git push origin feature/new-feature)
Open a Pull Request

## License
This project is licensed under the Apache 2.0 License.

## Contact
If you have any questions or suggestions, feel free to open an issue or contact me on LinkedIn.

## Project Structure:
nodejs/: Contains the NodeJS server code.
flutter/: Contains the Flutter app code.

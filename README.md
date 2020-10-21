node-red-contrib-iohook
========
# Description

Node for capturing keystrokes and mousestrokes.

# Installation

```bash
npm install node-red-contrib-io-hook

```

# Installation of dependency

```bash
npm install iohook

```

# Information

Simple node to catch key strokes on your keyboard and mouse.

Input: messages with msg.topic set to "state" with msg.payload true/false [boolean] are used to control
scanning of keyboard strokes and mouse clicks. Other messages are discarded.

Output: msg.topic is either "keyboard" or "mouse" following by msg.payload typeof number with number of keystroke or number of button clicked on mouse.<br>
When the control message is recieved, node sends message about changed state if command is correct with msg.topic "info".

![Example](https://raw.githubusercontent.com/lopikamper/node-red-contrib-io-hook/tree/main/images/example.png)


# What's new ?

* 0.1.2
  * Updated documentation
* 0.1.1
  * Now you can enable/disable node with msg.topic = "state"
  * Updated documentation
* 0.0.1
  * Published on npm and Node-RED flows

# Author

Copyright 2020 Bc. Jan Janovský

Faculty of Mechanical Engineering

Czech Technical University in Prague

# License
Apache-2.0

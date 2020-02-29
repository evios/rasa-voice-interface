# Rasa Voice Interface

A simple open source web interface for building voice assistants with
Rasa. The interface records the voice input by connecting to the microphone
enabled on your browser and autoplays the response generated by Rasa.

This is an alpha release of this voice interface. Community contributions
are very welcome.

### 🤖 How to install and run the Rasa voice interface

Necessary dependencies:
- node.js (https://nodejs.org)
- npm (https://www.npmjs.com/)


This is how you get the interface downloaded and ready to run:
```
git clone https://github.com/RasaHQ/rasa-voice-interface.git
cd rasa-voice-interface
npm install
```
And finally start the project with:
```
npm run serve
```

After that, the interface will start running on port 8080 and listen to port 5005. Launch
the voice interface by pointing your browser to https://localhost:8080.

### Which ASR systems can you use with this interface?
You can use this interface with any ASR systems you like. We tested this interface by 
integrating it with [Mozilla DeepSpeech](https://github.com/mozilla/DeepSpeech) and [Mozilla TTS](https://github.com/mozilla/TTS) components. A step-by-step implementation of this implementation
is documented here (https://blog.rasa.com/how-to-build-a-voice-assistant-with-open-source-rasa-and-mozilla-tools/).

### How to connect your Rasa assistant to this interface
To connect your own assistant to Rasa voice interface, you will need a connector. You can find an
example implementation of a custom connector in this tutorial. To adapt the interface to your 
project, you can change the welcome message by editing the `App.vue` and `store.js` files.


### Authors
Developed by [**INTEGR8**](https://www.integr8.com/) dev team, maintained by **Rasa**.


## :gift: License
Licensed under the Apache License, Version 2.0.
Copyright 2019 Rasa Technologies GmbH. [Copy of the license](LICENSE.txt).

# voice-to-text-JavaScript-project

![Screenshot (78)](https://user-images.githubusercontent.com/72680556/209417640-93659700-9592-4a90-90c6-80d102affbd5.png)

This project is a simple JavaScript library for converting speech to text using the Web Speech API.

# Getting Started
To use this library, you will need to include the voice-to-text.js file in your HTML file. Then, you can create a new instance of the VoiceToText class and start listening for speech.

***
<pre> 
<script src="app.js"></script>
<script>
  var vtt = new VoiceToText();
  vtt.startListening();
</script>
</pre>

***

![Screenshot (79)](https://user-images.githubusercontent.com/72680556/209417716-ec865546-73b1-47bf-8c17-b151e196e68a.png)

# Usage
To start listening for speech, call the startListening method on the VoiceToText instance. This will prompt the user to allow access to their microphone, and then start listening for speech.

***
<pre> 
vtt.startListening();
</pre>

***

***
<pre> 
vtt.stopListening();
</pre>

***

***
<pre> 
console.log(vtt.transcription);
</pre>

***

To stop listening for speech, call the stopListening method.

The VoiceToText class also has a transcription property that contains the latest transcription of the speech. You can access this property at any time to get the latest transcription.


# Limitations
The Web Speech API is supported in the latest versions of Google Chrome and Firefox, but is not supported in other browsers. This library will only work in those browsers.

Additionally, the accuracy of the transcription may vary depending on the quality of the microphone and the accent of the speaker.

# Credits
This library is based on the Web Speech API documentation from Mozilla Developer Network: https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API

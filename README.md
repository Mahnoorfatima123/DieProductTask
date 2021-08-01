Imagine a Single Page Web Application which is able to record spoken text as audio (mobile and desktop) and replay the recorded audio. The once recorded audio should be sent together with the email address of the user to a REST-API backend. 
The backend API receives the audio and asynchronously processes it by an algorithm which corrects potential (grammatical) errors and produces a corrected audio. Once the audio is corrected, the backend API sends it back to the frontend, where it is displayed and can be played back by the user. 

Frontend:
HTML5, CSS, REACT, Recorder.js, 
Backend:
PHP, Python, Google Speech Recognition API
Explanation:
I have kept frontend simple by using HTML5 and CSS for styling and used a plugin recorder.js to record the audio 
For backend , I have used PHP to make REST API and have used AJAX to send audio file as blob to backend server using XMLHttpService. Then I have used a stub Python Code of Google Speech Recognition API in an algorithm where speech recognition library is imported, than recognizer class is initialized in order to recognize the speech and than grammatical mistakes are corrected and audio is send back to the frontend using AJAX Get 
System Architecture:
Here quickly , I have used Client-Server Architecture where server hosts and delivers and manages the audio files , our frontend is the client and backend is the server where they both communicate in order to correctly deliver software.


Hello, I have a watch that sends its position via SMS by scanning nearby towers.
For this project, I've used node-red, Google Geolocation API and APP inventor
The main goal was to make it so the watch sends me its location on my phone, and the APP inventor I made take this message and use a broker to send it to node-red, then the message is parsed and the position is calculated thanks to Google Geolocation API and finally, the position is shown on a worldmap.
to make this work, you'll have to put your Google Geolocation API key in the "Prepare Geo request".
and you'll also have to set up your broker in MIT app inventor, I used this extension that allows MIT app inventor to handle mqtt requests :
https://ullisroboterseite.de/android-AI2-PahoMQTT-en.html
you'll just have to setup your broker in the Designer Tab

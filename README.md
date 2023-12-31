# Zoom-Clone-With-WebRTC
This is one of the best projects that I find in Kyle's WebDevSimplified page.
It uses very simple techniques to handle a video conference by using WebRTC.
But it can be updated in a way that it can be better.

for that I apply following changes.
1. Making server to be a HTTPS one instead of HTTP. In this way different web browsers from different computers can work with it. 
2. Change broadcast command to be like **socket.broadcast.to(roomId)**. It was **socket.to(roomId).broadcast** before.
3. Adding peer.js file locally. In this way, this project works without needing to be connected to Internet.
4. Adding Peer.js server localy to the server.js file. Now server.js brings the peer server up and running.
   But you need to install Peer.js package locally.It is added to package.json file now.
6. Adding a 500 ms delay before sending broadcast message to clients.

> **Note** Do not forget to add **https://**  before url in browsers, otherwise is does not work. It is a https server now.

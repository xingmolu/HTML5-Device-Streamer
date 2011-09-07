# HTML5-Device-Streamer

This is a simple demo of streaming live video from one web browser to another in Javascript.
 Video is captured using the mobile phone camera using getUserMedia(), periodically frames
 are captured and sent via a websocket to node.js which rebroadcasts them to all connected clients.
 The clients then show the video by rendering each frame as an image as it arrives. The framerate is
 slow due to the limited processor power of phones.

## Requirements

* An android phone running opera mobile with getUserMedia support - http://my.opera.com/ODIN/blog/2011/07/06/getusermedia-and-device-orientation-adventures
* A server running node.js to run the websocket server
* A websocket compatible browser to watch the video

## Inspiration

This quick hack was inspired by this video http://www.youtube.com/watch?v=cjmuwA8l1LQ 
but the author has not released the source anywhere I've found. As I had already been
 experimenting in the area I pretty much knew how to do it already
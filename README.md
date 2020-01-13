# vr-react
A VERY basic example of doing VR with React

I followed the tutorial here: https://pusher.com/tutorials/realtime-reactvr

Took me about 2 hours to build

# Compatablity Issue
Due to a known issue, you'll have to edit the blacklist file.

open file \node_modules\metro-bundler\src\blacklist.js

and change line 15 to:

var sharedBlacklist = [
  /node_modules[\/\\]react[\/\\]dist[\/\\].*/,
  /website\/node_modules\/.*/,
  /heapCapture\/bundle\.js/,
  /.*\/__tests__\/.*/
];;


# To Use:
* git clone https://github.com/mobeamer/vr-react.git
* cd vr-react/curr
* npm install
* make changes noted above to blacklist.js
* npm start

Open Browser: Http://localhost:8081/vr

The initial load takes a while, but you can edit the files on the fly from there on out.



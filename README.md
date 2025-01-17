# phaser-tcg

Separated version of client side and server side; on working.

Original code from DanZC.
A simple card game server using Node.js, socket.io, and Phaser.

The original code has many problems.
First, it was using Phaser2, not Phaser3.
Second, it was not separated client side and server side - client side and server side was referenced same files, which makes hard to understand the code. Even the code was written in object oriented aspect, the original code is totally a spaghetti.
Third, it was saving the data as class even on the server side. Server side should control the game only as data not as class; while client side should ask to change and react with change from the server on changing the data. This means, client only represents and asks the changes; server only controls the changes.

This repository is working to resolve those problems.

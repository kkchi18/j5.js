# j5.js
j5 scripts
 
 
 var five = require("johnny-five");
var board = new five.Board();

board.on("ready", function() {
 var led = new five.Led(13);
var motion = new five.Motion(2);

  motion.on("calibrated", function() {
    console.log("calibrated");
  });

  motion.on("motionstart", function() {
    console.log("motionstart");
	
  });

  motion.on("motionend", function() {
    console.log("motionend");
  });
  var led = new five.Led(13);
  
});  



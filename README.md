# Clock
For the clock that I created I wanted to have a little bit of fun and include a smiley face within my clock. For my clock the smallest line running through the smile of the smiley face represents the seconds on the clock. The slightly larger and different colored line within the smile represents the minutes of the clock. The largest line of the clock represents the hours of the day. The lines go from left to right counting down the minutes seconds and hours of the day. As all three of those run the eyes of the smile face are also counting time. The left eye represents days of the week while the right eye represents days of the year. I like this because on new years eve when the clock strikes midnight there will be nothing on the screen at the very point of new years and I will definintely be looking at this clock when new years comes around!

Here is where you can find my clock:
https://editor.p5js.org/jlane3/sketches/PfQxJhN0T

and here is my code for the clock:
function setup() {
  createCanvas(400, 400);
  angleMode(DEGREES);
}

function draw() {
  background(0);
  
  colorMode(RGB , 100)
  let hr = hour();
  let min= minute();
  let sec = second();
  let d= day();
  let y= year();
  
  strokeWeight(22)
  stroke(65, 50, 0)
  noFill()
  let end3 = map(hr, 0, 24, 180, 0);
  arc(200, 200, 300, 300, 0, end3);
  
  
  strokeWeight(8)
  stroke(25,25,0)
  noFill()
  let end2 = map(min, 0, 60, 180, 0);
  arc(200, 200, 300, 300, 0, end2);
  
  strokeWeight(4)
  stroke(200, 120 ,60)
  noFill()
  let end1 = map(sec, 0, 60, 180, 0);
  arc(200, 200, 300, 300, 0, end1);
  
  strokeWeight(10)
  stroke(200, 120 ,60)
  noFill()
  let end4 = map(d,0,7, 360, 0);
  arc(150,150,50, 50,0, end4);
  
  strokeWeight(10);
  stroke(200, 120 ,60)
  noFill()
  let end5 = map(y, 0, 365,180, 0);
  arc(250, 150, 50, 50, 0, end5);



  
 
  
 
 

  

  
}

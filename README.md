# ballsJS
Simple 2D balls, created with p5.js. Basic collision logic and mechanics

Take a look:
http://htmlpreview.github.io/?https://github.com/Meronkha/ballsJS/blob/master/bouncingball.html

What this project includes:
   -My own basic library containing basic vector functions (add,subtract, magnitude etc), you can check that out here:
    https://github.com/Meronkha/vectorJS
  
  -A function which can detect collisions between two objects:
  
  ```function distanceBetween(obj1,obj2){
  let temp = obj1.subtract(obj2)
  return temp.magnitude();
  }``
  
  This function will return the magnitude of the Vector between the two ball objects (their respective centres).
  The input of the function is two vector objects created using my own library mentioned before. 
  You can implement this function with the following code to generate collision detection:
  
  ```if (distanceBetween(ballVec1,ballVec2) < (myBalls[ballObj11].r/2 + myBalls[ballobj2].r/2)){
          // Insert appropriate response mechanism here```

Man-Zhu-s-Moving-Cat
====================

The assignment for Expressive Computation class

float x = 450;
float y = 200;

void setup(){
  size(500, 500);
  background(255);
  frameRate(30);
}
void draw(){
  background(255);
  smooth();
  noFill();
  stroke(0);
 
  fill(255,200,200);
  ellipse(x,y,30,30);//declare the ball
  
  beginShape();
  noFill();
  vertex(x+15,y);
  bezierVertex(x+20,y-30,x+30,y-80,x+50,y-100);
  bezierVertex(x+25,y-75,x+40,y-60,x+60, y-40);
  endShape();

fill(245,220,152);  
triangle(x-325,y-75,x-387.5,y-75,x-370,y-160);
triangle(x-325,y-75,x-262.5,y-75,x-300,y-160);

ellipse(x-100,y+50,300,30);
ellipse(x-200,y+30,230,200);

ellipse(x-340,y+50,40,200);//legs
ellipse(x-300,y+50,40,200);

fill(157,113,28);
ellipse(x-365,y+139,70,30);//brown feet
ellipse(x-270,y+139,70,30);

fill(245,220,152);//head
ellipse(x-325,y-75,125,125);

fill(255);//eye frame
ellipse(x-356.25,y-75,25,25);
ellipse(x-293.75,y-75,25,25);

fill(164,251,250);//eye ball
ellipse(x-356.25,y-75,10,25);
ellipse(x-293.75,y-75,10,25);

line(x-356.25,y-50,x-410,y-50);
line(x-356.25,y-40,x-410,y-40);
line(x-356.25,y-30,x-410,y-30);
line(x-293.75,y-50,x-240,y-50);
line(x-293.75,y-40,x-240,y-40);
line(x-293.75,y-30,x-240,y-30);

noFill();
line(x-325,y-60,x-325,y-40);
arc(x-340,y-40,30,30,0,PI/2.0);
arc(x-310,y-40,30,30,PI/2,PI);

fill(157,113,28);//brown foot
ellipse(x-180,y+120,100,40);

  x=x-3;
  y=y+3;
  if(y>500 && x<40){
    y=150;
    x=600;
  }  
}
 

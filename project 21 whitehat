
const Engine = Matter.Engine;
const World = Matter.World;
const Bodies = Matter.Bodies;
const Body = Matter.Body;
var ball, groundObj, rightobject, leftobject;
function preload()
{
	
}

function setup() {
	createCanvas(1600, 700);


	engine = Engine.create();
	world = engine.world;

	//Create the Bodies Here.

	var ball_options={
	isStatic:false,
	restitution:0.3,
	friction:0,
	density:1.2
}
ball=Bodies.circle(260,100,20,ball_options)
World.add(world,ball);

groundObj= new Ground(width/2,670,width,20);
leftobject= new Ground(1100,600,200,120);
rightobject= new Ground(1350,600,200,120);
	
Engine.run(engine);
  
}


function draw() {
  rectMode(CENTER);
  background(0);
  
  
  ellipse(ball.position.x,ball.position.y,40,40);
groundObj.display();
leftobject.display();
rightobject.display();

}



function keyPressed(){

if(keyCode===UP_ARROW){

Matter.Body.applyForce(ball,ball.position,{x:85,y:-85})	

}

	
}



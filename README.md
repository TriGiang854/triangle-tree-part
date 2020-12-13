async function startProgram() {
// This is our sample code for making the RVR drive in a triangle.
await drawTopTriangle(75)
await drawTopTriangle(75)


}

async function drawTopTriangle(speed){


await roll(55,speed,3.8) //Drive for 3.8 seconds at a speed of 75 at a heading of 55 degrees.
await stopRoll()
await roll(270,speed,5.6)//Continue for each corner of the triangle
await stopRoll()
await roll(128,speed,3.5)
await stopRoll()
//This realigns the robot at the end of the movement.

await roll(0,speed,0.5)


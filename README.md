# Drawing-Radar-Using-Processing-3

The values for the angle and the distance measured by the sensor will be read from the Arduino board by the Processing IDE using the SerialEvent() function which reads the data from the Serial Port. These values will be used for drawing the lines, the detected objects and some texts.

For drawing the moving lines we make this function drawLine(). Its center of rotation is set with the translate() function and using the line() function in which the iAngle variable is used to redraw the line for each degree 

For drawing the radar display we make this function drawRadar() which consist of arc() and line() functions.

For drawing the detected objects we made the drawObject() function. It receives the distance from the ultrasonic sensor, transforms it into pixels. Then, using the angle detected by the sensor it draws the object on the radar screen. 

To illustrate the text on the screen, we make the drawText() function that draws texts on some particular locations. All of these functions are called in the main draw() function which is repeated in each iteration to draw the screen details.

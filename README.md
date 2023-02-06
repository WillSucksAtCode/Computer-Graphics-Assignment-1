# Computer Graphics Assignment 1

Rim Lighting and Toon Ramp were created with shader graph's to work with URP
Rim lighting was created using the Fresnel Effect Node combined with a Color Node
Toon ramp was created with the help of this tutorial: https://www.youtube.com/watch?v=FIP6I1x6lMA

Game Build: htps://willidev.itch.io/viraldestructionnewbuild

Slide deck: https://docs.google.com/presentation/d/1Slj5Rv7sQssOBuobcQFC9AOYGcUwsKVYUcXjnqAx-eY/edit?usp=sharing  (I had issues with git)

Video Link: 

Demo Video: https://youtu.be/0nTK8nBbCEg

Video Transcript:
Hello! My name is William Heath, and this is my Assignment #1 for computer graphics.
Here is a photo of me, and my student number.

So, In this video, I’ll be going over 3 things, Toon ramp, Look Up Tables, and Rim Lighting.
Yeah I participated in a game jam over the weekend so I wasn’t able to implement everything and here we are.

To get us started, here is a video demonstrating all of the changes I added.

Next, for toon ramp.
I had to change it a bit for the shader to work in Unity’s Render Pipeline, but, the main idea behind how a toon ramp works is that you get the dot product between the normal of the surface and the direction of the light. Then we multiply that value by 0.5 and add 0.5, and use that value along with our ramp texture to give us the cool look that toon ramp has. The final value, which can be anything from 0-1, is used to pick which shade of the ramp texture that specific normal should use.

For the Look Up Tables, I was unable to get them to work on our characters camera, possibly because of cinemachine or some other plugin in the project, but I still created the LUT’s regardless. Which I did in photoshop.

Finally, we have Rim Lighting.
Rim lighting is done by getting the view direction of the user, and then getting the dot product of the that and the normal of the object, saturating it, and subtracting that value by 1. You can then modify this with color or an intensity float.

And unfortunately, that is all I have to showcast today, thank you for watching.

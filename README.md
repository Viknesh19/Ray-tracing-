Ray tracing is a rendering technique that simulates the path of light and intersections with objects and is able to produce images with a high degree of realism.

The scene that is to be rendered is abstracted into a set up consisting of the following components: objects, in a 3D space, a light source, a camera or an eye, and a screen (Figure 1):  
<img width="831" height="604" alt="image" src="https://github.com/user-attachments/assets/925638ec-cc6a-4b4f-99fc-722a1501a29b" />

Figure 1

In ray tracing, the process of real-life illumination has been simplified to include only rays that pass through the screen. In reality, light rays come out of the light source in all directions, bounce on objects and then hit the eye. However, since not all rays emitted from the light source will end up in the eye, ray tracing does the reverse process to save computation time where rays are traced from the eye back to the light source. This backward tracing is shown below in Figure 2:

<img width="505" height="396" alt="image" src="https://github.com/user-attachments/assets/91925e5d-2594-4ae9-b143-613c08b0582a" />

Figure 2

Setting up the scene

When setting up the scene, we need to decide where the camera and the screen are located. To make things simple, the camera and the screen are aligned with unit axis (Figure 3).

<img width="518" height="482" alt="image" src="https://github.com/user-attachments/assets/51699f2a-a663-487f-aee8-f1270b57ba36" />

Figure 3


The camera is located at the point (x=0, y=0, z=1) and the screen is part of the plane formed by the x and y axes.

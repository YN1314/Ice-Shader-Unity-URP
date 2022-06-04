![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Thumbnail.jpg)

## Overview
An ice shader with fake cracks depth and depth texture transparency (you can see outlines of other objects below the ice).

### How does fake depth work?
Basically, the shader samples a cracks texture multiple times. Each sample slightly changes the UV based on the tangent space's view direction.
In the end, the shader combines the cracks texture and combined color of all samples. I know it sounds kinda confusing (*because it is!*), so please check the code in ***Assets/Shaders/tojynick/Ice/HLSL/Ice Depth.hlsl***
### Notice
The more samples the shader does, the slower it runs. So be careful with *Samples* setting, especially on mobile devices.

## Important Notes
### Compatibility
The shader is tested only in **Unity 2021** and only with **URP**, so I cannot guarantee it will work properly in earlier versions of Unity or different render pipelines.
### URP Settings
Please make sure **Depth Texture** is enabled. Otherwise you will not be able to see objects below the ice.

## Examples
[YouTube Video](https://www.youtube.com/watch?v=hIEWdt4ALn0)

### GIFs
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Ground.gif)
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Cubes.gif)

### Screenshots
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Ground%201.jpg)
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Sphere.jpg)

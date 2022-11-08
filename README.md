![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Thumbnail.jpg)

## Overview ℹ️
An ice shader with fake cracks depth and depth texture transparency (you can see outlines of other objects below the ice).

### How does fake depth work?
The shader is using a technique called **Parallax Mapping**. Basically, it samples the cracks multiple times. Each sample it slightly changes the UV based on the tangent space's view direction. It gives the illusion of depth.

I know it sounds kind of confusing (*because it is!*), so please check the code in *Assets/Shaders/Library/HLSL/Ice Depth.hlsl* or you can read more about Parallax Mapping [here](https://en.wikipedia.org/wiki/Parallax_mapping).

### Notice
The more samples the shader does, the slower it runs. So be careful with *Samples* setting, especially on mobile devices.

## Important Notes ⚠️
### Compatibility
The shader is tested only in **Unity 2021** and only with **URP**, so I cannot guarantee it will work properly in earlier versions of Unity or different render pipelines.
### URP Settings
Please make sure **Depth Texture** is enabled. Otherwise you will not be able to see objects below the ice.

## Examples 👀
### GIFs
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Ground.gif)
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Cubes.gif)

### Screenshots
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Ground%201.jpg)
![alt text](https://github.com/tojynick/Ice-Shader/blob/main/Readme%20Resources/Ice%20Sphere.jpg)

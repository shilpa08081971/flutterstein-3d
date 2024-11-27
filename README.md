Original README.md:

# Flutterstein 3D

A 3D raycaster implemented in Flutter.

> For anyone looking for the _original / unminified_ code, there is a branch named `prior-to-reduction` which is pretty much the code prior to the minification.
 
> This app was submitted as an entry to the [Flutter 5KB Challenge](https://flutter.dev/create).

![Gameplay 0](/captures/gameplay0_320x180.gif?raw=true)
![Gameplay 1](/captures/gameplay1_320x180.gif?raw=true)
![Gameplay 2](/captures/gameplay2_320x180.gif?raw=true)
![Gameplay 3](/captures/gameplay3_320x180.gif?raw=true)

## Description

This is a an implementation of the 3D raycasting algorithm as employed by games like Wolfenstein 3D. It uses the Canvas API, specifically `drawRawAtlas`, to render the level data and also to batch the draw calls.

On-screen controls have also been implemented using `PointerData`, with _inflated_ tap areas to improve responsiveness.

> ### To keep things interesting
>
> Due to the 5KB restriction, I can't really add any game logic. However, when I built the level, I hid 9 other Flutter logos (10 if you count the first logo at the start) within the level, see if you can find them all before reaching the exit (the exit is another _elevator_).
>
> If you want to see where all of the logos are hidden, [here is the map](/captures/level_map.png?raw=true)

## Running the app

```bash
flutter run --release
```

I highly recommend running this on _Android_ devices since that is where I have been testing the app on. Theoretically, it should also run on iOS since there is no platform specific code or configuration employed.

> ### Orientation
>
> Although the app supports both _portrait_ and _landscape_ orientation, it looks way better in _landscape_.

README.md After SOme Improvements & Migration To The Currently Latest FLutter Version: 3.24.5 In Channel: Stable:

Explanation
Modernized Code:
The code is now more readable and maintainable.
Null safety and type annotations are used for better type checking. Modern Dart features like async/await are used for asynchronous operations.

Future Roadmap Visualized:

Enhanced Features:
The game now uses Flutter's experimental Flutter GPU and Flutter Scene features, functionalities, implementations & integrations for better performance and rendering. Advanced 3D packages like ditredi, zflutter, and flutter_cube can be integrated to add more advanced 3D features. New game mechanics, such as more complex raycasting, lighting, and shading, are implemented.

Optimization:
The code is optimized for better performance, especially on mobile devices. Flutter's performance profiling tools are used to identify and fix bottlenecks.

Testing:
The game is tested on multiple devices and platforms to ensure compatibility and performance. Unit and integration tests are written using Flutter's testing framework. Documentation and Community Engagement:
The README.md file is updated with detailed documentation. The project is shared on social media and developer communities to encourage contributions and feedback.

Possible Integrations:
Integrate Advanced 3D Packages:
Interoperability With flutter_3d_raycast_engine:
3D Raycast Engine in Flutter, using DDA(Digital Differential Analyzer) Algorithm.
&
Add support for 3D models and textures using packages like flutter_3d_obj and flutter_cube. Implement more advanced lighting and shading using ditredi and zflutter.

Optimize and Test:
Use Flutter's performance profiling tools to further optimize the game. Test the game on a variety of devices and platforms.

Community Engagement:
Share the project on social media and developer communities. Encourage contributions and feedback from the community. By following these steps, you can modernize and enhance the Flutter 3D ray casting game engine to take full advantage of the latest Dart and Flutter features and technologies.

Known Issues:

![390483020-692f7135-84a6-437c-a782-9df0e6676a33](https://github.com/user-attachments/assets/08dc2490-b254-4a96-86c2-5beca4711627)

The discrepancy in output quality between the two debug builds of Flutter's Web WASM and Windows is notable. The Web WASM debug build, displayed on the left, appears significantly lower in quality, with an unwanted level of pixelation compared to the Windows debug build. On the right, the Windows debug build presents a much sharper and clearer image. This contrast raises questions about the underlying causes of such drastic differences in rendering between the two platforms.

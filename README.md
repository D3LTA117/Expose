# Expose
One of my slides that I created myself on Unreal Engine 4 for my presentations at the university. This is just a tech demo.

Keyboard shortcut :
- Next : space
- Previous : backspace
- Menu : escape

![Infiltrator Demo Screenshot 2023 08 13 - 19 45 51 94](https://github.com/D3LTA117/Expose/assets/73521232/e2f628f4-94fb-4a3c-b4c7-963086fb898c)


![Infiltrator Demo Screenshot 2023 08 13 - 19 46 03 63](https://github.com/D3LTA117/Expose/assets/73521232/b0f5bffd-0a55-49cd-8257-e53c9a5dee86)

There are 2 graphics options, "PC de la NASA" (ultra quality) and "minitel de mami" (low quality). I have locked framerate to 120 fps because high-end configs are too powerful.

List of graphic config :



Both :
- Vsync : on
- Chromatic aberation : off
- Ambiant occlusion : off
- Depth of field : off
- Shadows : off
- Lens flare : off
- Refraction : off
- Screen space reflection : off
- Light function : off
- Show FPS : on



PC de la NASA :
- Antialiasing : temporal antialiasing
- Temporal antialiasing for upslampling : on
- View distance : cinematic
- Screen percentage (supersampling) : 200%
- Eye adaptation : high
- Bloom : ultra
- Tonemapper : grain quantization
- Max anisotropy : 16
- Motion blur : ultra



Minitel de mami :
- Antialiasing : off
- Temporal antialiasing for upslampling : off
- View distance : 0
- Screen percentage (supersampling) : 70%
- Eye adaptation : off
- Bloom : off
- Tonemapper : off
- Max anisotropy : 0
- Motion blur : off


For my code, I use Blueprint.

Total view of my Blueprint level code.

![total view](https://github.com/D3LTA117/Expose/assets/73521232/b2d3f4c5-4ab2-4a4c-8800-e111be8bfb07)

- First, I initialize game controller and view for the user and I lock movement.

![initialyze](https://github.com/D3LTA117/Expose/assets/73521232/5633a2d6-1c5e-4ef0-b8fe-ca1192c5d0ae)

- Second, I open automatically the main menu with graphics options and I block the keyboards shortcut.

![main menu](https://github.com/D3LTA117/Expose/assets/73521232/cd6800f4-eb94-4ebe-8f32-0d9d6e7f2854)

- Third, I create a Matinee template with events trigger where animation stops on each one.

![matinee](https://github.com/D3LTA117/Expose/assets/73521232/6f02c411-75dd-4253-a66a-99ff393308e4)

- Forth, I create keyboards shortcut for Matinee with next and previous slide.

![keyboard](https://github.com/D3LTA117/Expose/assets/73521232/e1ba4a49-a36c-4e32-9f43-547f78522ab3)

- Fifth, I close my Blueprint level with the main menu keyboard shortcut.

![escape](https://github.com/D3LTA117/Expose/assets/73521232/a0a22e96-557e-4027-b626-3f74d548c595)

- Sixth, in my main menu widget, I create buttons for graphics option and quit application. I apply modify graphic in terms of what user want, close widget and giveback keyboard shortcut to the user.

![widget](https://github.com/D3LTA117/Expose/assets/73521232/ac3358c6-7e11-43e9-aa17-d515161e2668)

- Seventh, quit button trigger.

![quit](https://github.com/D3LTA117/Expose/assets/73521232/3d7cb4d2-733b-4d4a-a9b8-4e0aace12f15)

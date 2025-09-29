## Compiling the Project Locally
Here is a zip file with all files needed to compile my project on windows:
[project1Graphics.zip](https://github.com/user-attachments/files/22585764/project1Graphics.zip)
Extract these zip files to a new folder, and open that folder in windows Terminal or command prompt.
To compile, you must have SDL3 downloaded to the computer, which you can get from [here](https://github.com/libsdl-org/SDL/releases/latest.). Download "
SDL3-devel-3.2.22-VC.zip ", and extract the files to a folder of your choosing (C:\*yourSDLfilepath\*). I extracted the files to a new folder with the location "C\SDL".
On my computer, I can compile the project by running the following line in the command prompt:
```
g++ .\squareStarter.cpp .\glad\glad.c -I C:\SDL\SDL3-3.2.22\include -L C:\SDL\SDL3-3.2.22\lib\x64 -lSDL3 -o project1.exe
```
You want to change "C:\SDL\SDL3-3.2.22\include" and "C:\SDL\SDL3-3.2.22\lib\x64" to have the correct file path on your computer, so this will look like:
```
g++ .\squareStarter.cpp .\glad\glad.c -I C:\*yourSDLfilepath*\SDL3-3.2.22\include -L C:\*yourSDLfilepath*\SDL3-3.2.22\lib\x64 -lSDL3 -o project1.exe
```
This should compile a new executable "project1.exe".

## Running the project/Extra Features
While in the project directory, type "project1.exe" into the command line. Pressing "g" will change the texture of the square between the three textures given in the project starter code.

# Aseductor
- A simple batch script to compile aseprite automatically with just copying and pasting so that you can do your work while the work is being done in the background
- I've come up with idea of making this script for a long time now as I see lots of people suffering in an attempt to compile Aseprite (like me). It took me a (whole) week to compile the program myself that's why I wanna help people
- I am not good at using batch so I searched google for 70% of the code :D

# Setup

**Tutorial**: https://youtu.be/gsPpLAgT-iI 
<br>
(Recommend combining both reading and watching video to stay updated)
<br>
<br>Remember to read https://github.com/Perndoe/Aseductor#notes

- Install Visual Studio and dependencies as mentioned in https://github.com/aseprite/aseprite/blob/main/INSTALL.md#dependencies
  + Add ninja.exe to C:\Program Files\Ninja then add C:\Program Files\Ninja\ninja.exe to Path
  + Add C:\Program Files\CMake\bin to Path
  + If you don't know how to then check https://gist.github.com/nex3/c395b2f8fd4b02068be37c961301caa7
  + Check the video to make things easier
- Install Skia and Aseprite source code (Aseprite any versions)
  + https://github.com/aseprite/aseprite/releases
  + https://github.com/aseprite/skia/releases
- Put Skia and Aseprite in a folder in Downloads named "Compressed"
- Create a folder named "Skia Windows" and a folder named "Aseprite" in "Compressed"
  + In "Skia Windows" create a new folder named "skia" then extract skia release files there
  + In "Aseprite" extract Aseprite source code in

**Important**
- I'll make a video for new updates (when I am free) if you can't find it here
- Only extract the source code inside those zip files

# Compilation
- Install the latest version of the script: https://github.com/Perndoe/Aseductor/releases
- Run the script as Administrator so that it'll copy the files to C:\\
- **To make sure it work well, here are 2 ways of compiling**
  - Need Internet: (The process will take a bit longer than manually setting up)
    + You don't need to install Aseprite source code yourself (Skia is still required)
    + After opening the script, a browser tab will pop up. Find the Aseprite version you wanted and copy its link address
    + Then paste into the script window. It will install "asepritesc.zip" in "Downloads\Compressed" folder so don't delete it by yourself
    + Only use this method if you don't want to download Aseprite source code and set it up yourself
    <br> ![image](https://github.com/Perndoe/Aseductor/assets/81963564/48c0c6af-b4ae-441a-9a52-0c0fd617ce68) 
    <br> (Currently copying "Aseprite-v1.3-rc4-Source.zip" link address)
    <br>
    
  - No Internet
    + You must prepare and set up as shown in https://github.com/Perndoe/Aseductor/edit/main/README.md#setup
    + After opening the script, close the browser tab that open at the start and type "skip" into the command prompt. You will see some errors but it is fine

- The script automatically compiles Aseprite to C:/aseprite/build/bin so if the script didn't open File Explorer, you can find it yourself
- Keep "data" folder and "aseprite.exe" in "bin" and you can remove the 3 other files
- You must delete the "deps" and the "aseprite" folder in "C:/" after finish compiling if you have already moved the "bin" folder out
- Keeping "Skia Windows" folder for future updates is recommended

# Compilation & Deleting caches
- Install "Aseductor.DelCache.bat" from https://github.com/Perndoe/Aseductor/releases
- After Aseprite is compiled, the script will move the program to Desktop/Compiled Aseprite
- It will delete these files after compiling:
  + C:\deps
  + C:\aseprite
- Make sure there is no folder in Desktop named "Compiled Aseprite" if you use this script

# Notes
- As I don't have a Mac computer, I can't really make a Mac version, sincerely sorry :(
- Don't worry if you can't find the "Aseprite" folder in "Compressed" after compiling :D
- If the compilation failed, rewatch my video, follow step by step or get help through **Issues** tab: https://github.com/Intrivus/Aseductor/issues
- Links for commands that I don't know: 
  + https://stackoverflow.com/questions/4619088/windows-batch-file-file-download-from-a-url
  + https://stackoverflow.com/questions/21704041/creating-batch-script-to-unzip-a-file-without-additional-zip-tools
  + https://stackoverflow.com/questions/24546150/how-can-prevent-a-powershell-window-from-closing-so-i-can-see-the-error
  + https://stackoverflow.com/questions/28481915/how-to-make-chat-bot-in-batch
  + https://stackoverflow.com/questions/26223936/open-a-web-page-in-a-windows-batch-file
  + https://stackoverflow.com/questions/19422604/batch-script-for-renaming-and-then-moving-files-from-1-folder-to-another
  + https://stackoverflow.com/questions/16502283/how-do-i-fix-access-denied-with-the-move-command-in-windows-7

## OpenCV C++ Development on Apple Silicon Macs using VS Code ##
*19 November 2023*

This is based on project is based on `Elliotcodes` YouTube video `How to Setup OpenCV for C++ on Visual Studio Code (MacOS)` https://youtu.be/Ozc3zWJ_NhQ?si=kJsDgmfhg79IAQvg. This project adds a few bits which make using OpenCV or any other modern C++ project easier on the Mac.

* It uses the still experimental but nonetheless excellent CMake extension for VS Code. (Version is 0.0.17 at time of writing)
    * CMake does all of the grunt work of finding libraries that you have installed. You don't have to create and configure `tasks.json` or `c_cpp_properties.json`.
* It includes a video and it is of me of course, talking about Android development in 2012.

### Install Software ###

1. You should have the following already installed on your Mac:
    1. Xcode, from Mac App Store, ` -> App Store`
    1. Be sure to install Xcode command line extensions.
        1. Open the Terminal app and enter:
        1. `xcode-select --install`
    1. Homebrew: go to `https://brew.sh/`
    1. Use brew to install:
        1. cmake, `brew install cmake`
        1. pkg-config, `brew install pkg-config`
        1. opencv, `brew install opencv`
    1. Visual Studio Code: go to `https://code.visualstudio.com/download`

### Install Essential Extensions: ###

* Main Tools
    * C/C++
    * C/C++ Extension Pack
    * C/C++ Themes
    * CMake Tools
    * CMake
* Check each extension to be sure it is `Enabled`.

### Install Optional Extensions: ###

* Docker and Remote Tools (Not needed for this app but useful to have)
    * Dev Containers
    * Docker
    * Remote - SSH
    * Remote - SSH: Editing Configuration Files
    * Remote Explore

### Building, Debugging, and Running ###
1. CMake: Select a Kit,
    1. Select: Clang 13.0.0
    1. This will create a build folder
1. CMake: Select a Variant
    1. Select Debug (typical while developing)
1. CMake: Configure
1. Build 

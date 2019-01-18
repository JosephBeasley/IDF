# Using an IDE

For this lesson, we are going to dive into using IDEs to debug. The IDEs we will be using are **CLion** and **Visual Studio**. Both are outstanding and powerful debuggers. 

![](/assets/clion.png)

* **License:** Proprietary
* **Platforms:** Windows, OSX, Linux
* **Price:** $89 1st year (monthly payments and free/dicounted accounts avaliable)
* Truly cross-platform (full functionality on all platforms)
* Intelligent autocompletion engine
* Utilizes CMake and other system tools for building
* Can use LLVM (Clang) or GCC compiler
* Easy to setup
* Powerful refactoring
* Faster than Intellisense
* Large amount of plugins
* Powerful debugger
* Code analysis
* We will be using this on Linux

![](/assets/vs.png)

* **License:** Proprietary
* **Platforms:** Windows, OSX, Linux (limited functionality on OSX/Linux)
* **Price:** Paid/Free (Community version is free)
* Intellisense (Very powerful auto completion, peaking, etc)
* Good range of plugins
* Integrated well with Windows
* Pretty simple
* Ironed Out
* Utilizes MSBuild tools
* We will be using this on Windows

---
---
---


## Why use an IDE?

There are many reasons to use an IDE over a text editor... even one with plugins such as `Visual Studio Code`, `Atom` or `Sublime Text Editor`. The reasons become more apparent as the project grows in size and complexity. 

1. Code highlighting, syntax validation, auto code formatting and auto completion. Sure, many of the above text editors have that functionality. But you can be sure the above IDEs implement that functionality much better. Especially when we are talking about projects with multiple files.
2. Debugging: This is arguably the biggest reason. Text Editors with plugins have the ability to debug... but it's rather limited. With Visual Studio and CLion... you can dive into assembly, static analysis, dynamic analysis, memory, peak, stack trace, watch values, etc. 
3. Compiling and managing lib dependencies: On large projects... you may need to set a compile order of files, manage lib dependencies, handle cleanup, etc. Sure, you can create scripts to do this. But it can become overwelming. IDEs can do it for you and save you a bunch of time. 
4. Result Preview: IDEs generally handle your final result previews better. This also includes the creation of GUIs. 
5. Refactoring and performance hints: IDEs can help you refactor code across the entire project in one or two steps. IDEs can also provide hints on how to increase the performance of your project. 
6. Inspecting Code: IDEs allow for the inspection of code as you are programming. This helps a ton when dealing with libs.
7. Documentation: IDEs often include tools to assist in documentation... even doing it for you sometimes. 
8. Team tools: IDEs include and can utilize plugins to streamline the team development process.


---

# IDE Basic Use

The first step to using an IDE is to create a new project. We are very briefly going to go over how to do this in the markdown. The instructor will give you a more in-depth live preview. 

## CLion

1. Open CLion
2. Click `New Project`
3. For our C Programs, choose `C Executable` using the C99 standard
4. Give your project a name, our project is called `myProject`
5. Click Create

![](/assets/clion_new.png)

You will then be presented with a window. Two files will have been created: `CMakeLists.txt`. This file is what configures CMake to make and build our project. There is also our `main.c` file. This is our entry point for our project... at least in relation to programming in C. 

![](/assets/clion_project_window.png)

There are multiple `tool windows` within the standard CLion workspace that we need to discuss. 

#### Project Window

This window will contain all of our files, External Libraries, etc. We are mostly interested with whats inside of the `myProject` dir. (This will be named whatever you named your project). Expanding that, we see the cmake file, the .c file and a dir called `cmake-build-debug`. All of the executables, debugging files, etc go here.

* [More info](https://www.jetbrains.com/help/clion/project-tool-window.html)

![](/assets/clion_window.png)

We can then right click `myProject` and we will be presented with an array of choices. 

* To create new dirs, click `Directory`
    * This should create a link on the CMake file. If it doesn't... manually add it. 
* To create new C sources files, click `C/C++ Source File`
    * This should create a link on the CMake file. If it doesn't... manually add it. 
    * Ensure you select the correct language type (C)
* To create new C header files, click `C/C++ Header File`
    * This should create a link on the CMake file. If it doesn't... manually add it. 
    * Ensure you select the correct language type (C)

![](/assets/clion_rclick.png)

#### Code Window

This window is the very large window in which you will be writing your code. 

#### Run/Debugging Bar

This bar is a quick and graphical representation of the Build and Run dropdown menus. 

* Clicking the green right arrow will run your code. Output will be displayed in the output/terminal window which will appear below the code window. 
* Clicking the green bug will put your program into debugging mode. 
* The other buttons are useful, but we will not discuss it in the markdown. 
* If you click the `run` dropdown menu, you will see these same choices.
* If you click the `build` dropdown menu, there is some additional functionality avaliable. 
    * `Rebuild Project` will rebuild your project. Even if you didn't make any changes. 
    * `Clean` will clean the project by building the clean target from the current CMake profile
    * [More Info](https://www.jetbrains.com/help/clion/build-actions.html)

![](/assets/run_bar.png)

#### Terminal/CMake/TODO Window

This window will show your output in the terminal (if any), any errors, CMake information and any TODOs you create. 

* To create a TODO, you simply type `// TODO:` as a comment. 

![](/assets/clion_term.png)


### More Info on Getting Started with CLion

[CLion - Getting Started](https://www.jetbrains.com/help/clion/clion-quick-start-guide.html)



---
---
---

## Visual Studio

### More Info on Getting Started with Visual Studio

Sadly, the offical Visual Studio getting started guide is down. So we will link a third party. 

[Visual Studio - Getting Started](https://www.cs.auckland.ac.nz/~paul/C/Windows/index.php)



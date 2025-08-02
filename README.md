# libvultra-starter-template
A starter template for rapidly creating graphics or game prototypes with libvultra.

## Examples
Please see [here](https://github.com/zzxzzk115/libvultra/tree/master/examples).

## Build Instructions

Prerequisites:
- Git
- XMake
- Vulkan SDK
- Visual Studio with MSVC if Windows
- GCC or Clang if Linux/Unix
- XCode with GCC or Apple Clang if macOS

Step-by-Step:

- Install XMake by following [this](https://xmake.io/guide/quick-start.html#installation). 

- Clone the project:
  ```bash
  git clone https://github.com/zzxzzk115/libvultra-starter-template.git
  ```

- Build the project:
  ```bash
  cd libvultra-starter-template
  # xmake f --wayland=n # disable wayland, fallback to x11
  # xmake f --wayland=y # enable wayland
  # xmake f -m debug # prepare to build debug
  # xmake f -m release # prepare to build release
  xmake -vD
  ```

- Run the program:
  ```bash
  xmake run
  ```

  > **Tips:**
  > For OpenXR programs, you may need to set the XR_RUNTIME_JSON environment variable.
  > For debugging OpenXR programs without headsets, you may need Meta XR Simulator on Windows and macOS. On Linux, you can use Monado as the simulator.

## License
This project is under the [MIT](LICENSE) license.

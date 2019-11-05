# Install Vulkan and the necessary GAME dependencies on your Linux distribution
### Firstly, support for 32-bit libraries: is required for the main software used, such as WINE and GAMES.

##### For Arch Linux and derivatives (Arch Labs, Artix, Manjaro and etc) just run the command below exactly as follows, this will not only install the vulkan driver, but will improve performance on 2d designer software, 3d and also in GAMES:

```
sudo pacman -Syy --noconfirm egl-wayland eglexternalplatform libglvnd glfw-wayland clinfo opencl-headers opencl-mesa intel-opencl-clang libclc ocl-icd lib32-ocl-icd lib32-libglvnd lib32-glu glu libva-mesa-driver mesa mesa-demos mesa-vdpau lib32-mesa lib32-mesa-demos lib32-mesa-vdpau lib32-smpeg lib32-sdl_ttf lib32-sdl_mixer lib32-sdl_image lib32-sdl2_ttf lib32-sdl2_mixer lib32-sdl2_image lib32-sdl2 lib32-sdl sdl sdl2 sdl2_image sdl2_mixer sdl2_ttf sdl_image sdl_mixer sdl_ttf smpeg lib32-openal gambas3-gb-openal alure openal-examples openal freealut ffnvcodec-headers libxnvctrl xf86-video-nouveau nvidia-cg-toolkit steam-native-runtime lib32-gtk3 vulkan-devel attr lib32-attr fontconfig lib32-fontconfig lcms2 lib32-lcms2 libxml2 lib32-libxml2 libxcursor lib32-libxcursor libxrandr lib32-libxrandr libxdamage lib32-libxdamage libxi lib32-libxi gettext lib32-gettext freetype2 lib32-freetype2 linux-headers dkms libsm lib32-libsm gcc-libs lib32-gcc-libs libpcap lib32-libpcap desktop-file-utils giflib lib32-giflib libpng lib32-libpng gnutls lib32-gnutls libxinerama lib32-libxinerama libxcomposite lib32-libxcomposite libxmu lib32-libxmu libxxf86vm lib32-libxxf86vm libldap lib32-libldap mpg123 lib32-mpg123 openal alsa-lib lib32-alsa-lib libxcomposite lib32-libxcomposite mesa-libgl lib32-mesa-libgl opencl-icd-loader lib32-opencl-icd-loader libxslt lib32-libxslt libpulse lib32-libpulse libva lib32-libva gtk3 gst-plugins-base-libs lib32-gst-plugins-base-libs vulkan-icd-loader lib32-vulkan-icd-loader sdl2 lib32-sdl2 vkd3d lib32-vkd3d gsm ffmpeg xf86-video-ati xf86-video-amdgpu xf86-video-intel xf86-video-nouveau libva-intel-driver libva-utils libva-vdpau-driver libva1 libva1-intel-driver vulkan-intel libgphoto2 ncurses lib32-ncurses libjpeg-turbo lib32-libjpeg-turbo lib32-alsa-plugins vulkan-radeon lib32-vulkan-intel lib32-vulkan-radeon lib32-vulkan-validation-layers wine-staging
```

##### For UBUNTU and DERIVATIVES commands may vary depending on the version and distribution you use and it is recommended to use recent versions of your distro:

```
sudo apt-get update

sudo apt-get install wget dialog libnotify

sudo apt-get install libc6:i386

sudo apt-get install ia32-libs

sudo dpkg --add-architecture i386

sudo apt-get install wine32-development

sudo apt-get install mesa-vulkan-drivers vulkan-utils libassimp4 libvulkan1

sudo apt-get install dxvk dxvk-wine32-development dxvk-wine64-development libvkd3d-dev libvkd3d-utils1 libvkd3d1 libvulkan-dev libvulkan1 mesa-vulkan-drivers renderdoc vkd3d-demos vulkan-tools vulkan-utils vulkan-validationlayers vulkan-validationlayers-dev winehq-staging
```

##### For FEDORA and DERIVATIVES the commands may vary depending on the version and distribution used and it is recommended to use recent versions of your distro:
```
sudo dnf -y install dnf-plugins-core

dnf config-manager --add-repo https://dl.winehq.org/wine-builds/fedora/30/winehq.repo

sudo dnf -y install winehq-staging wget dialog libnotify
```

##### Second. Boost performance with +50 FPS - enable Esync.
https://tuninglinux.github.io

##### Third. Make sure your Vulkan driver is enabled. For Plastas Nvidia, simply install the proprietary driver. For AMD RADEON boards, follow this tutorial below:
https://amdgpu.github.io/

[![Vamos_aos_Jogos](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/vamos_aos_jogos.gif)](https://github.com/felipefacundes/PlayOnGit-en)

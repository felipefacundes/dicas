# Instale o Vulkan e às dependências necessárias para JOGOS na sua distribuição Linux
### Primeiro saiba que é o suporte as aplicações 32 bits. São necessários para os principais softwares utilizados, como o WINE e JOGOS.


##### Para Arch Linux e derivados (Arch Labs, Artix, Manjaro e etc) basta executar o comando abaixo exatamente da forma como se segue, isso não só instalará o driver vulkan, como melhorará o desempenho em softwares de designers 2d, 3d e também em JOGOS:

```
sudo pacman -Syy --asdeps egl-wayland eglexternalplatform libglvnd glfw-wayland clinfo opencl-headers opencl-mesa intel-opencl-clang libclc ocl-icd lib32-ocl-icd lib32-libglvnd lib32-glu glu libva-mesa-driver mesa mesa-demos mesa-vdpau lib32-mesa lib32-mesa-demos lib32-mesa-vdpau lib32-smpeg lib32-sdl_ttf lib32-sdl_mixer lib32-sdl_image lib32-sdl2_ttf lib32-sdl2_mixer lib32-sdl2_image lib32-sdl2 lib32-sdl sdl sdl2 sdl2_image sdl2_mixer sdl2_ttf sdl_image sdl_mixer sdl_ttf smpeg lib32-openal gambas3-gb-openal alure openal-examples openal freealut ffnvcodec-headers libxnvctrl xf86-video-nouveau nvidia-cg-toolkit steam-native-runtime lib32-gtk3 vulkan-devel attr lib32-attr fontconfig lib32-fontconfig lcms2 lib32-lcms2 libxml2 lib32-libxml2 libxcursor lib32-libxcursor libxrandr lib32-libxrandr libxdamage lib32-libxdamage libxi lib32-libxi gettext lib32-gettext freetype2 lib32-freetype2 glu lib32-glu linux-headers dkms libsm lib32-libsm gcc-libs lib32-gcc-libs libpcap lib32-libpcap desktop-file-utils giflib lib32-giflib libpng lib32-libpng gnutls lib32-gnutls libxinerama lib32-libxinerama libxcomposite lib32-libxcomposite libxmu lib32-libxmu libxxf86vm lib32-libxxf86vm libldap lib32-libldap mpg123 lib32-mpg123 openal lib32-openal v4l-utils lib32-v4l-utils alsa-lib lib32-alsa-lib libxcomposite lib32-libxcomposite mesa lib32-mesa mesa-libgl lib32-mesa-libgl opencl-icd-loader lib32-opencl-icd-loader libxslt lib32-libxslt libpulse lib32-libpulse libva lib32-libva gtk3 lib32-gtk3 gst-plugins-base-libs lib32-gst-plugins-base-libs vulkan-icd-loader lib32-vulkan-icd-loader sdl2 lib32-sdl2 vkd3d lib32-vkd3d sane libgphoto2 gsm ffmpeg samba xf86-video-ati xf86-video-amdgpu xf86-video-intel xf86-video-nouveau libva-intel-driver libva-utils libva-vdpau-driver libva1 libva1-intel-driver vulkan-icd-loader vulkan-intel vulkan-radeon lib32-vulkan-icd-loader lib32-vulkan-intel lib32-vulkan-radeon lib32-vulkan-validation-layers python-olefile python-pyqt5 xorg-server xorg-server-devel
```

##### Para UBUNTU e DERIVADOS:

```
sudo dpkg --add-architecture i386

sudo apt-get install dxvk dxvk-wine32-development dxvk-wine64-development libvkd3d-dev libvkd3d-utils1 libvkd3d1 libvulkan-dev libvulkan1 mesa-vulkan-drivers renderdoc vkd3d-demos vulkan-tools vulkan-utils vulkan-validationlayers vulkan-validationlayers-dev winehq-staging
```

##### Segundo. Certifique-se que o seu driver Vulkan está habilitado. Para plascas Nvídia, basta instalar o driver proprietário. Para placas RADEON da AMD, siga esse meu tutorial abaixo:
https://amdgpu.github.io/

##### Terceiro. Aumente a performance com mais +50 de FPS - habilite o Esync.

```bash
su -c 'echo -e "* hard nofile 1048576" >> /etc/security/limits.conf'
su -c 'echo -e "vm.swappiness=0" > /etc/sysctl.conf'
reboot
```

[![Vamos_aos_Jogos](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/vamos_aos_jogos.gif)](https://github.com/felipefacundes/PlayOnGit)

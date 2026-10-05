# PythonReverseEngineering


```
┌──(kali㉿kali)-[~/…/Reverse_Engineering/Htb/rev_tinyplatformer/TinyPlatformer_extracted]
└─$ ls
base_library.zip                libSDL2-2-d6813302.0.so.0.14.0       pygame
FreeSansBold.ttf                libSDL2_image-2-554041b7.0.so.0.2.3  pyiboot01_bootstrap.pyc
libbz2.so.1.0                   libSDL2_mixer-2-5dc902ba.0.so.0.2.2  pyimod01_os_path.pyc
libcrypto.so.1.0.0              libSDL2_ttf-2-dd80ed71.0.so.0.14.1   pyimod02_archive.pyc
lib-dynload                     libssl.so.1.0.0                      pyimod03_importers.pyc
libffi.so.6                     libtiff-97e44e95.so.3.8.2            pyimod04_ctypes.pyc
libFLAC-bf6d1292.so.8.3.0       libtinfo.so.5                        pyi_rth_inspect.pyc
libfreetype-2d39c124.so.6.17.1  libuuid.so.1                         pyi_rth_pkgres.pyc
libjpeg-bd53fca1.so.62.0.0      libvorbis-205f0f59.so.0.4.8          pyi_rth_pkgutil.pyc
libmikmod-fabcac29.so.2.0.4     libvorbisfile-f207f3a6.so.3.3.7      pyi_rth_subprocess.pyc
libogg-b51fbe74.so.0.8.4        libwebp-582c46b3.so.7.1.0            PYZ-00.pyz
libpng16-b14e7f97.so.16.37.0    libz-a147dcb0.so.1.2.3               PYZ-00.pyz_extracted
libpython3.7m.so.1.0            libz.so.1                            struct.pyc
libreadline.so.6                main.pyc
```

```
┌──(kali㉿kali)-[~/…/Reverse_Engineering/Htb/rev_tinyplatformer/TinyPlatformer_extracted]
└─$ pycdc main.pyc
# Source Generated with Decompyle++
# File: main.pyc (Python 3.7)

import pygame
import os
import sys

def resource_path(relative_path):
    base_path = getattr(sys, '_MEIPASS', os.path.dirname(os.path.abspath(__file__)))
    return os.path.join(base_path, relative_path)

pygame.init()
(WIDTH, HEIGHT) = (800, 640)
PLAYER_SIZE = 40
SCROLL_AMOUNT = 520
GRAVITY = 0.8
JUMP_ACCEL = 15
........
```


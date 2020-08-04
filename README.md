# GIF decoder for LVGL
Allow to use of GIF images in LVGL from. 

Based on https://github.com/lecram/gifdec

Compatible with LVGL's `feat/new-fs-api` branch. 
If you use the [lv_fs_if](https://github.com/lvgl/lv_fs_if) repository its `new-api` branch should be used.


## Get started
- Download or clone this repository
  - [Download from GitHub](https://github.com/lvgl/lv_lib_gif/archive/master.zip)
  - Clone: `git clone https://github.com/lvgl/lv_lib_gif.git`
- Include the library: `#include "lv_lib_gif/lv_gif.h"`

## Use GIF images from file
```c
lv_obj_t * img = lv_gif_create_from_file(parent, "S/path/to/img.gif");
```

## Use GIF images from flash
If the gif file stored in the flash as a C array: 
```c
lv_obj_t * img = lv_gif_create_from_data(parent, gif_data);
```



# How to Update Firmware

To update firmware, please follow the procedure below:

#### **Step 0**: Install the flash programming tool before updating.
Download the [dloader](https://github.com/unisoc/dloader/releases/download/unisoc-v0.3.1/dloader_0.3.1-1_amd64.deb) and install it.

```shell
  sudo dpkg -i dloader_0.x.x-1_amd64.deb
```

In addition, you can build the dloader.

```shell
  make dloader
```

#### **Step 1**: Switch bootstrap pin to ROM Code mode.
  ┌──────────────┐
  │ ┌─┐   ┌─┐┌─┐ │
  │ │O│ O │O││O│ │
  │ ├─┤┌─┐├─┤├─┤ │
  │ │O││O││O││O│ │
  │ └─┘├─┤└─┘└─┘ │
  │  O │O│ O  O  │
  │    └─┘       │
  └──────────────┘

#### **Step 2**: Power on the board, and execute the following sequence of commands:

```shell
  cd output/repeater/images
  ./update_fw.sh
```

#### **Step 3**: Switch bootstrap pin to NOR Flash mode again and push the reset button.
  ┌──────────────┐
  │    ┌─┐┌─┐┌─┐ │
  │  O │O││O││O│ │
  │ ┌─┐├─┤├─┤├─┤ │
  │ │O││O││O││O│ │
  │ ├─┤└─┘└─┘└─┘ │
  │ │O│ O  O  O  │
  │ └─┘          │
  └──────────────┘

To update one image or several images, please refer to help of ```update_fw.sh```.

```shell
  ./update_fw.sh -h
```


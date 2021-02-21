# Xmodmap Configuration
After using the MacBook for a while, I realized that the key behavior and the mouse scrolling was more natural in MacOS. For that reason, I reconfigure my keyboard modifier into MacOS look-alike.

## What is this config file do?
* Remap modifier keys on Linux.
  - [Left Control] as [Left Win/Super]
  - [Left Win/Super] as [Left Alt]
  - [Left Alt] as [Left Control]
  - [Right Alt] as [CapsLock]

## Usage:
Just copy `.Xmodmap` to home directory (`~/`) or we can use this command below:
```bash
cp .Xmodmap ~/
```

The next step is to restart the computer. Or we can start it immediately using this command below:
```bash
xmodmap ~/.Xmodmap
```

#### Note:
We can have multiple keyboard layout configuration by creating another `.Xmodmap` files, for example `.Xmodmap-AnnePro` as I reconfigure it for my AnnePro keyboard.
```bash
setxkbmap -option # for resetting xmodmap configuration
xmodmap ~/.Xmodmap-AnnePro
```

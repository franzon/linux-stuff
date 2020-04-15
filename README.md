# Some stuff to make Ubuntu work

## GRUB config for Nvidia

```bash
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash acpi_osi=Linux-Dell-Video alx.enable_wol=1 mem_sleep_default=deep nouveau.modeset=0"
```

## Keyboard media keys freezing

1. `sudo nano /usr/share/X11/xkb/symbols/br`
2. Search for `modifier_map Mod3   { Scroll_Lock };`
3. Comment this line
4. Restart

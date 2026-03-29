# grub-theme-synth

A simple grub theme inspired by synthwave aesthetics.

I created this theme back in 2023, when I was refurbishing one of my old laptops as a retrogaming rig that had to multi-boot Batocera and Debian.

Icons are based on `candy-icon-theme`.

## How to install it

1. Clone this repo:

```bash
git clone https://github.com/manu-creative-411/grub-theme-synth.git
```

2. Move the directory somewhere in your disk:

```bash
sudo mkdir -p /boot/grub/themes
sudo mv grub-theme-synth /boot/grub/themes/synth
```

⚠️ Have a second look on the final path. You will need it on the next step.

3. Config `grub` to use the theme:

```bash
sudo nano /etc/default/grub
```

```
# ADD/EDIT THIS LINE AND SET THE CORRECT PATH FOR THE THEME'S theme.txt:
GRUB_THEME=/boot/grub/themes/synth/theme.txt
```

4. Save, exit and update `grub`

```bash
sudo update-grub # Debian/Ubuntu
# or
sudo grub2-mkconfig -o /boot/grub2/grub.cfg # Fedora
```

5. Reboot. That's all.

#!/usr/bin/env bash

sudo pacman -Syu --noconfirm
sudo pacman -S --needed --noconfirm \
    git qt5-base qt5-multimedia xorg noto-fonts-emoji polkit ttf-opensans \
    make alsa-utils kwindowsystem python3 xcompmgr upower \
    openbox xorg-xinit xterm lxappearance-gtk3 arc-gtk-theme
mkdir -p "$HOME/.config/openbox"
if [ ! -f "$HOME/.config/openbox/rc.xml" ]; then
    cp /etc/xdg/openbox/{rc.xml,autostart,environment} "$HOME/.config/openbox/"
fi
echo "exec openbox-session" > "$HOME/.xinitrc"
sh -c "$(curl -fsSL plainde.github.io/install)"
cat << 'EOF' >> "$HOME/.config/openbox/autostart"

# plainDE Components
plainPanel &
plainControlCenter --tray &
xcompmgr -c &
EOF

echo "=== Setup complete!!! ==="
echo "Just type startx and enjoy!!"
echo "by ThatFatKeker"

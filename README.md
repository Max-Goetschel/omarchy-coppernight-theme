<div align="center">

# 🌌 Omarchy: Copper Night

> *"Where the deep indigo of Tokyo meets the warm glow of an ember sunset."*

A high-performance **Hyprland** rice for Omarchy featuring a custom **Tokyo Night** palette accented by a striking **Copper-Orange** border.

![Version](https://img.shields.io/badge/version-1.0-orange?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)
![Hyprland](https://img.shields.io/badge/Hyprland-Rice-indigo?style=for-the-badge&logo=archlinux)

</div>

---

## 📸 Preview

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a9805426-69f0-4d69-8b51-d0b8654c22a8" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/55a73042-3a03-4afa-abce-12ded1ce1ac1" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/22a14853-7611-4216-a146-50e6b7a63e85" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1401f0f0-706e-4ce9-8a08-2befff95aba9" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/df4535c4-f46f-4977-9d0c-e6a6f6e99881" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2092b281-3c01-4997-806f-88c1d608c313" />
---

| **Feature** | **Description** |
|:---|:---|
| 🖼️ **Wallpaper** | Traditional Japanese Pixel Art Pagoda. |
| 🪟 **UI** | Floating diagnostic widgets with custom resource bars. |
| 🎨 **Colors** | Deep Indigos, Magentas, and Copper-Orange accents. |

---

## 🚀 Easy Installation (One-Line)

This command installs all system dependencies (Python libraries, NetworkManager, and Papirus Icons), performs a safe backup of your existing Waybar config, and applies the Copper Night theme.

```bash
sudo pacman -S --needed python-requests python-psutil networkmanager papirus-icon-theme && \
omarchy-theme-install https://github.com/hembramnishant50-glitch/omarchy-coppernight.git && \
{ [ -d ~/.config/waybar ] && mv ~/.config/waybar ~/.config/waybar-backup-$RANDOM; }; \
mkdir -p ~/.config/waybar && \
cp -r ~/.config/omarchy/themes/coppernight/waybar/. ~/.config/waybar/ && \
chmod +x ~/.config/waybar/scripts/* && \
gsettings set org.gnome.desktop.interface icon-theme 'Papirus-Dark' && \
killall waybar; waybar &

# Grub Theme Expedition 33

A GRUB boot theme inspired by the video game *Clair Obscur : Expedition 33*.

## Preview

A quick preview of how the theme will look on your computer :
<video src="https://github.com/user-attachments/assets/41dd813f-e97f-4676-ac74-c59b7cd6f5b8" controls="controls" width="100%"></video>

---

## Installation

### rerequisites
Make sure GRUB2 is installed on your system (this is the default on the vast majority of Linux distributions).

### Manual Method

1. **Clone the repository** (or download it as a .zip and extract it):
   ```bash
   git clone [https://github.com/Ayayyyaaa/grub-theme-expedition33.git](https://github.com/Ayayyyaaa/grub-theme-expedition33.git)
   cd grub-theme-expedition33
   ```

2. **Copy the theme folder** to the GRUB themes directory (requires root privileges):
   ```bash
   sudo mkdir -p /boot/grub/themes/
   sudo cp -r expedition33 /boot/grub/themes/
   ```

3. **Edit the GRUB configuration** :
   Open the GRUB config file with your favorite text editor (nano, vim, gedit...):
   ```bash
   sudo nano /etc/default/grub
   ```

4. **Modify the GRUB settings** :
   Look for the line starting with `GRUB_THEME=`. If it doesn't exist, add it at the end of the file:
   ```ini
   GRUB_THEME="/boot/grub/themes/expedition33/theme.txt"
   ```
   *(Also make sure to uncomment or add `GRUB_TERMINAL_OUTPUT="gfxterm"` if it's not already there. For the best experience, you can also set your resolution with `GRUB_GFXMODE="1920x1080"`).*

5. **Update GRUB** :
   To apply the changes, update GRUB depending on your distribution:
   
   * **Ubuntu / Debian / Linux Mint:**
     ```bash
     sudo update-grub
     ```
   * **Arch Linux / Fedora / others:**
     ```bash
     sudo grub-mkconfig -o /boot/grub/grub.cfg
     ```
     *(Check the exact path to your grub.cfg. On some EFI systems like Fedora, it might be `/boot/efi/EFI/fedora/grub.cfg`).*


## Credits & License

* Theme created by Ayayyyaaa.
* Inspired by the universe of *Clair Obscur: Expedition 33* (Sandfall Interactive).
* Distributed under the License.
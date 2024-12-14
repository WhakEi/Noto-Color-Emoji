# Noto Color Emoji
للعربية (إضغط هنا)[https://github.com/WhakEi/Noto-Color-Emoji/blob/master/README-AR.md]

This fork of Noto Color Emoji replaces the old Syrian Flag with the New one following the collapse of the Dictator Bashar al-Assad.

## Installation Instructions
### Linux

1. Download the font file from releases
2. Move the font file to `/usr/share/fonts/`
(If you installed a distro with preinstalled emoji support, remove the existing Noto Color Emoji file and skip to step 6)
4. If it doesn't already exist, create a file in `/etc/fonts/local.conf`
5. Add the following text to said file
```
<?xml version="1.0"?>
<!DOCTYPE fontconfig SYSTEM "urn:fontconfig:fonts.dtd">
<fontconfig>
    <alias>
        <family>sans-serif</family>
        <prefer>
            <family>Noto Color Emoji</family>
        </prefer>
    </alias>

    <alias>
        <family>serif</family>
        <prefer>
            <family>Noto Color Emoji</family>
        </prefer>
    </alias>

    <alias>
        <family>monospace</family>
        <prefer>
            <family>Noto Color Emoji</family>
        </prefer>
    </alias>
</fontconfig>
```
6. Refresh system fonts using the `fc-cache` command

### Windows
1. Download `seguiemj.ttf` from releases
2. Press Start+R and type `Shell:fonts`
3. Scroll down until you find "Segoe UI Emoji"
4. Right click it, go to Properties
5. Go to Security tab, click Advanced, change the owner of the file to your Windows username
6. Go back to Security properties, click Edit this time, find your Users and select Full Control
7. Right click the font and delete it
8. Now go to the `seguiemj.ttf` file you downloaded, right click it (click "Show More Options" if you're on W11) and click "Install for all users".
9. Restart

### Android
1. Download `NotoColorEmoji.ttf` from releases
2. Download zFont 3 from Play Store
3. Go to "Downloads" tab, click the + button and choose "Add File"
4. Add the file you downloaded
5. Name it whatever you want
6. Follow the instructions on the app (Varies by phone manufacturer)

### macOS
While it seems to be possible, it requires a lot of effort and messing with system files, so this is still being worked on.

### iOS
Unfortunately as of right now it seems impossible to change emoji fonts on iOS and iPadOS devices **even with jailbreak**.

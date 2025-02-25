Firstly, I want to say that I used my own installation of Android Studio for the example.
So run the command below:
```bash
nano $HOME/.local/share/applications/androidstudio.desktop
```
Where `androidstudio` can be the name of your application.
the content within this *.desktop file must basically contain the data below:
```bash
[Desktop Entry]
Name=Android Studio
Type=Application
Exec=/home/username/.android/android-studio/bin/studio
Icon=/home/username/.android/android-studio/bin/studio.png
```

Below is a more complete form, and if your installation was within `/opt` for example:
```bash
[Desktop Entry]
Version=1.0
Name=Android Studio
Comment=IDE for Android Development
Exec=/opt/android-studio/bin/studio.sh %f
Icon=/opt/android-studio/bin/studio.png
Terminal=false
Type=Application
Categories=Development;IDE;
```

And that's it!

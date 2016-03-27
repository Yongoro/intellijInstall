# Intellij IDEA Installation on linux environment

## Get the zip and install it

* download link: 

  * https://www.jetbrains.com/idea/download/#section=linux
  
* unzip the file into destination path
```
  tar -xzvf ideaIC-2016.1.tar.gz -C /opt
```
## Executable file creation
```
touch /usr/bin/IDEA
 
chmod 755 /usr/bin/IDEA
```

## Use your favourite text editor and paste the following lines

* file creation using vim
```
vim /usr/bin/IDEA
```
* paste the following lines
```
#!/bin/sh
export IDEA_HOME="/opt/idea-IC-145.258.11/bin"

$IDEA_HOME/idea.sh $*
```
## Desktop entry creation

* file creation
```
vim /usr/share/applications/IDEA.desktop
```
* paste the following lines 
```
[Desktop Entry]
Encoding=UTF-8
Name=intellj IDEA
Comment=Intellij IDEA IDE
Exec=IDEA
Icon=/opt/idea-IC-145.258.11/bin/idea.png
Terminal=false
Type=Application
Categories=GNOME;Application;Development;
StartupNotify=true
```
## call your IntelliJ IDEA

```
IDEA
```

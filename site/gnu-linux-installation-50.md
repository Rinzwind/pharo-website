title: Download - GNU/Linux installation (50)
sudo apt-get update
sudo apt-get install ia32-libs
 sudo apt-get update 
 sudo apt-get install libx11-6:i386 
 sudo apt-get install libgl1-mesa-glx:i386 
 sudo apt-get install libfontconfig1:i386 
 sudo apt-get install libssl1.0.0:i386 
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install pharo-vm-core
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install pharo-launcher
# which is then used like this:
pharo /path/to/your/image
# which is then launched via:
pharo-launcher
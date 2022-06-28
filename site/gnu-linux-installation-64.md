title: Download - GNU/Linux installation - 64bits
$ yum-config-manager --add-repo http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/CentOS_6/devel:languages:pharo:stable.repo

# Install 32bit packages (with X11 dependency for *-ui or not) 
$ yum install pharo6-32-ui.i686 or pharo6-32.i386 

# Install 64bit packages 
$ yum install pharo6-64-ui.x86_64 pharo6-64.x86_64 
$ cd /usr/lib64
$ ln -s libcurl.so.4 libcurl-gnutls.so.4

# Add the repo 
$ yum-config-manager --add-repo http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/CentOS_7/devel:languages:pharo:stable.repo

# Install 64bit packages
$ yum install pharo6-64-ui.x86_64 pharo6-64.x86_64 
$ wget -O - http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/Debian_8.0/Release.key | apt-key add - 

#add repository
echo "deb http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/Debian_8.0/ ./" > /etc/apt/sources.list.d/pharo.list 

# Update and install 
$ apt update 
$ apt install pharo6-32-ui pharo6-64-ui    (or pharo6-32 or pharo6-64) 
$ wget -O - http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/xUbuntu_14.04/Release.key | apt-key add - 

#add repository
echo "deb http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/xUbuntu_14.04/ ./" > /etc/apt/sources.list.d/pharo.list 

# Update and install 
$ apt update 
$ apt install pharo6-32-ui pharo6-64-ui 
$ wget -O - http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/xUbuntu_16.04/Release.key | apt-key add - 

#add repository
echo "deb http://download.opensuse.org/repositories/devel:/languages:/pharo:/stable/xUbuntu_16.04/ ./" > /etc/apt/sources.list.d/pharo.list 

# Update and install 
$ apt update 
$ apt install pharo6-32-ui pharo6-64-ui 
# or if curl is not available:
wget -O- https://get.pharo.org/64 | bash
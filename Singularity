Bootstrap: docker
From: ubuntu:19.04

%post
    apt-get -y update
    apt-get -y install fortune cowsay lolcat
    apt-get -y install python3
    git clone astfast

%environment
    export LC_ALL=C
    export PATH=/usr/games:$PATH

%runscript
    fortune | cowsay | lolcat
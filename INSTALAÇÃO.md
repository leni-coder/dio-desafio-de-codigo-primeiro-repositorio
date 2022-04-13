#Para Instalação Do Git no Linux Deve-se fazer o Seguinte:


* Deve-se saber qual é a distribuição instalada no pc;


#Aqui Será Desmonstrado Os Comandos Para Apenas Algumas Distribuições:

#Debian/Ubuntu
Para a versão estável mais recente para o seu lançamento do Debian/Ubuntu

apt-get install git
Para o Ubuntu, este PPA fornece a versão mais recente do Git upstream estável

add-apt-repository ppa:git-core/ppa # apt update; apt install git
#Fedora
 yum install git(até Fedora 21)

dnf install git(Fedora 22 e posterior)

#Gentoo
emerge --ask --verbose dev-vcs/git

#Arch Linux
pacman -S git



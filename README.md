## Tutorial sobre como instalar o Octoprint no Raspberry e no Linux Debian

## Linux
Tutorial da comunidade do Octoprint bem detalhado sobre como instalar no Raspbian. Este tutorial discorre sobre duas formas de instalar. A primeira refere-se à instalação utilizando uma imagem a ser colocada num cartão SD. A segunda é uma instalação a partir de um Linux, com criação do ambiente virtual, instalação do Python e usando pip:
[Setting up OctoPrint on a Raspberry Pi running Raspberry Pi OS (Debian)](https://community.octoprint.org/t/setting-up-octoprint-on-a-raspberry-pi-running-raspberry-pi-os-debian/2337)
Atentar para a necessidade de alterar a permissão do arquivo /etc/systemd/system/octoprint.service com chmod +x .
Atentar ainda que o arquivo tem um atributo para o usuário e que ele tem que ser o usuário da instalação do Octoprint

[Install Octoprint on Linux – Complete Guide! - Detalhamento para instalar a câmera](https://3dprintscape.com/install-octoprint-on-linux/)


Tutorial sobre como instalar o Octoprint diretamente a partir da imagem do Raspi OS com a imagem do Octopi embutida:
[How to setup OctoPrint! + best plugin recommendations](https://youtu.be/HBd0olxI-No?t=374)

Tutorial sobre suporte à webcam e timelapse no Octoprint: [Using ffmpeg for webcam streaming and timelapse support](https://community.octoprint.org/t/using-ffmpeg-for-webcam-streaming-and-timelapse-support/5321)

Video detalhado do canal de Chris Riley sobre a instalação do Octoprint no Linux:
[![Octoprint On Linux - Install - How To - Chris's Basement](http://i3.ytimg.com/vi/fimVwRXarf4/hqdefault.jpg)](https://www.youtube.com/watch?v=fimVwRXarf4)

Atenção especial à descrição no video no Youtube. Há vários links para todas as ferramentas que são usadas no vídeo.

Nova forma de instalar no Linux com link para batch no github
(https://octoprint.org/download/)

## Instalar Python 3.9.9 sobre a versão nativa do Linux 1.08 LTS que é a 3.6.9
Verifique se você possui o pip instalado executando o seguinte comando:
````
python3.6 -m pip --version
````

````
sudo apt update
sudo apt install python3-pip
````

````
sudo apt remove python3.6
````

````
sudo apt install build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev tk-dev
````

````
wget https://www.python.org/ftp/python/3.7.12/Python-3.9.9.tar.xz
````

````
tar -xf Python-3.9.9.tar.xz
````

````
cd Python-3.9.9
````

````
./configure --enable-optimizations
````

````
make -j$(nproc)
````



````
sudo make altinstall
````

### ou se quiser subressvrever a versão nativa
````
sudo make install
````

````
python3.7 --version
````



Tutorial completo da 3D Printscape com video. O video aponta para esse arquivo e o arquivo tem o link do video
[Install Octoprint on Linux – Complete Guide!](https://3dprintscape.com/install-octoprint-on-linux/)


Video ótimo sobre o Rescuezila: (https://www.youtube.com/watch?v=NvZa_PsKjLU&t=672s)


## Windows
Tutorial da comunidade do Octoprint sobre a instalação no Windows: [Setting up OctoPrint on Windows](https://community.octoprint.org/t/setting-up-octoprint-on-windows/383)









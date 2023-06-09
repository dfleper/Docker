# Installing Docker on Ubuntu or Linux Mint

![GitHub repo size](https://img.shields.io/github/repo-size/dfleper/Docker?logo=github)
![GitHub last commit](https://img.shields.io/github/last-commit/dfleper/Docker?color=blue&label=last-commit&logo=github&logoColor=white)

##### Installing Docker on Ubuntu 20.04 Focal or Linux Mint 20.2 Uma. 
##### Instalación de Docker en Ubuntu 20.04 Focal o Linux Mint 20.2 Uma.

##### Open the terminal Ctrl+Alt+T. Copy and Paste + Return. 

<a href="https://www.docker.com/" target="_blank"> <img src="https://www.docker.com/wp-content/uploads/2022/03/vertical-logo-monochromatic.png" alt="Docker" width="48" height="48"/> </a> 

```
sudo apt-get update
```
```
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg
```
```
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
```
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  focal stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```
sudo apt-get update
```
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
```
sudo docker run hello-world
```
-----

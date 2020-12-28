# Запуск

```bash
docker run -v "путь-до-id_rsa.pub":/root/.ssh/_authorized_keys -p 22:22 -d --name mf y2khub/mainframer
```

# Установка docker на elementary OS

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc

sudo apt-get update

sudo apt-get -y install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo apt-add-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"

sudo apt-get update
sudo apt-get -y install docker-ce
```

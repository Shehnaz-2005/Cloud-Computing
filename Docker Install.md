# Docker Install
### Install Packages:
```
sudo apt update
sudo apt install -y \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
    jq
```
### Add Docker’s Official GPG Key:
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
### Setup Repository:
```
echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
### Install Docker Engine:
```
sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io
```
### Add Your User to the Docker Group:
```
sudo usermod -aG docker $USER
```
### Download the Current Stable Release of Docker Compose:
```
COMPOSE_VERSION=$(curl -s "https://api.github.com/repos/docker/compose/tags" | jq -r '.[0].name')
sudo curl -L "https://github.com/docker/compose/releases/download/${COMPOSE_VERSION}/docker-compose-$(uname -s)-$(uname -m)" \ o /usr/local/bin/docker-compose
```
### Apply Executable Permissions to the Binary:
```
sudo chmod +x /usr/local/bin/docker-compose
```

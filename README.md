# Docker
# Installing Docker On Ubuntu #
## For installing docker use these following commands ##

**update packages**
```
sudo apt update 
```
## Install Prerequisites ##
```
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
```
## Add Docker GPG Key
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
## Set Up the Stable Docker Repository
```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
## Install Docker Engine
```
sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io
```

# GenAI-Assistant
## 1. Create Aws ec2 medium instance with 20gb stroage
### 2.	Sudo apt update
### 3.	Create virtual environment 
cd /backend
```
sudo apt install –y python3 python3-pip-venv
python venv/bin/activate
source venv/bin/activate

```
### 4.	install node
```
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 22

# Verify the Node.js version:
node -v # Should print "v22.14.0".
nvm current # Should print "v22.14.0".

# Verify npm version:
npm -v # Should print "10.9.2".
```
### 5. create .env file in backend directory
cd /backend
```
OPEN_API_KEY:sksvcacctdh4ECyHYy0oZRiFc2vmBn0s2xHvwSJNXQly2M1L0fTwFD90lD1UgKHeSSBxo2GPSc50CX2yTLT3BlbkFJopihJ5WwNWSYwyLMZhquZ_I1rvSM7Q3tRLetXuZCfVMh7uBVPk2ns9FEVlcQAwB4OxHtrLkwA
-important note : download new api key
```
### 6. create .env file in frontend directory
cd /frontend

```
NEXT_PUBLIC_API_BASE_URL=http://backend:8000
```
### 7. install 
Cd /backend

```
pip install –r reuirement.txt
uvicorn main:app --reload --host 0.0.0.0 --port 8000

```
### 8. install npm
```
npm install
npm run dev 
```
# for Dockerization
### 1.	install docker
```
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
	"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
	$(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
	sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo usermod -aG docker Ubuntu
newgrp
```
### 2.	install docker-compose
```
sudo curl -SL https://github.com/docker/compose/releases/download/v2.35.0/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

```

### 3.	docker-compose up
```
docker-compose up
```
### 4. Run npm
cd /frontend
```
npm run build
```









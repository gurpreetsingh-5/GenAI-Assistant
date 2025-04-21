# GenAI-Assistant
## 1. Create Aws ec2 medium instance with 20gb stroage
### 2.	Sudo apt update
### 3.	Create virtual environment 
```
	sudo apt install –y python3 python3-pip-venv
	cd /backend
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

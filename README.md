📋 Individual Commands with Copy Buttons
1️⃣ System Update & Node.js Installation
<details> <summary>Click to expand commands</summary>
bash
# Update system
sudo apt update && sudo apt upgrade -y
<button onclick="copyToClipboard('sudo apt update && sudo apt upgrade -y')">📋 Copy</button>

bash
# Install curl
sudo apt install curl -y
<button onclick="copyToClipboard('sudo apt install curl -y')">📋 Copy</button>

bash
# Install Node.js
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
<button onclick="copyToClipboard('curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -')">📋 Copy</button>

bash
# Complete Node.js installation
sudo apt install -y nodejs
<button onclick="copyToClipboard('sudo apt install -y nodejs')">📋 Copy</button>

bash
# Verify installation
node -v && npm -v
<button onclick="copyToClipboard('node -v && npm -v')">📋 Copy</button>

</details>
2️⃣ Project Directory Setup
<details> <summary>Click to expand commands</summary>
bash
# Create project directory
sudo mkdir -p /var/www
<button onclick="copyToClipboard('sudo mkdir -p /var/www')">📋 Copy</button>

bash
# Navigate to directory
cd /var/www
<button onclick="copyToClipboard('cd /var/www')">📋 Copy</button>

</details>
3️⃣ GitHub SSH Configuration
<details> <summary>Click to expand commands</summary>
bash
# Generate SSH key
ssh-keygen -t ed25519 -C "tawhidulislam3482@gmail.com" -f ~/.ssh/id_ed25519 -N ""
<button onclick="copyToClipboard('ssh-keygen -t ed25519 -C "tawhidulislam3482@gmail.com" -f ~/.ssh/id_ed25519 -N ""')">📋 Copy</button>

bash
# Start SSH agent
eval "$(ssh-agent -s)"
<button onclick="copyToClipboard('eval "$(ssh-agent -s)"')">📋 Copy</button>

bash
# Add SSH key
ssh-add ~/.ssh/id_ed25519
<button onclick="copyToClipboard('ssh-add ~/.ssh/id_ed25519')">📋 Copy</button>

bash
# Show public key
cat ~/.ssh/id_ed25519.pub
<button onclick="copyToClipboard('cat ~/.ssh/id_ed25519.pub')">📋 Copy</button>

bash
# Test GitHub connection
ssh -T git@github.com
<button onclick="copyToClipboard('ssh -T git@github.com')">📋 Copy</button>

</details>
4️⃣ Clone & Setup Project
<details> <summary>Click to expand commands</summary>
bash
# Clone repository
git clone YOUR_REPO_URL
<button onclick="copyToClipboard('git clone YOUR_REPO_URL')">📋 Copy</button>

bash
# List contents
ls
<button onclick="copyToClipboard('ls')">📋 Copy</button>

bash
# Enter project folder
cd YOUR_PROJECT_FOLDER
<button onclick="copyToClipboard('cd YOUR_PROJECT_FOLDER')">📋 Copy</button>

bash
# Install dependencies
npm i
<button onclick="copyToClipboard('npm i')">📋 Copy</button>

bash
# Build project
npm run build
<button onclick="copyToClipboard('npm run build')">📋 Copy</button>

</details>
5️⃣ Firewall Configuration
<details> <summary>Click to expand commands</summary>
bash
# Install firewall
sudo apt install ufw -y
<button onclick="copyToClipboard('sudo apt install ufw -y')">📋 Copy</button>

bash
# Allow SSH
sudo ufw allow 22
<button onclick="copyToClipboard('sudo ufw allow 22')">📋 Copy</button>

bash
# Allow HTTP
sudo ufw allow 80
<button onclick="copyToClipboard('sudo ufw allow 80')">📋 Copy</button>

bash
# Allow HTTPS
sudo ufw allow 443
<button onclick="copyToClipboard('sudo ufw allow 443')">📋 Copy</button>

bash
# Allow your app port
sudo ufw allow 3000
<button onclick="copyToClipboard('sudo ufw allow 3000')">📋 Copy</button>

bash
# Enable firewall
sudo ufw --force enable
<button onclick="copyToClipboard('sudo ufw --force enable')">📋 Copy</button>

</details>
6️⃣ PM2 Setup
<details> <summary>Click to expand commands</summary>
bash
# Install PM2
npm i -g pm2
<button onclick="copyToClipboard('npm i -g pm2')">📋 Copy</button>

bash
# Start app with PM2
pm2 start npm --name "YOUR_APP_NAME" -- start
<button onclick="copyToClipboard('pm2 start npm --name "YOUR_APP_NAME" -- start')">📋 Copy</button>

bash
# View logs
pm2 logs YOUR_APP_NAME
<button onclick="copyToClipboard('pm2 logs YOUR_APP_NAME')">📋 Copy</button>

bash
# List all processes
pm2 ls
<button onclick="copyToClipboard('pm2 ls')">📋 Copy</button>

bash
# Save PM2 processes
pm2 save
<button onclick="copyToClipboard('pm2 save')">📋 Copy</button>

bash
# Setup startup script
pm2 startup
<button onclick="copyToClipboard('pm2 startup')">📋 Copy</button>

</details>
🔄 Re-deployment Commands
<details> <summary>Click to expand commands</summary>
bash
# Navigate to project
cd /var/www/YOUR_PROJECT_FOLDER
<button onclick="copyToClipboard('cd /var/www/YOUR_PROJECT_FOLDER')">📋 Copy</button>

bash
# Pull latest changes
git pull
<button onclick="copyToClipboard('git pull')">📋 Copy</button>

bash
# Install dependencies
npm i
<button onclick="copyToClipboard('npm i')">📋 Copy</button>

bash
# Build project
npm run build
<button onclick="copyToClipboard('npm run build')">📋 Copy</button>

bash
# Check running processes
pm2 ls
<button onclick="copyToClipboard('pm2 ls')">📋 Copy</button>

bash
# Restart app
pm2 restart APP_ID_OR_NAME
<button onclick="copyToClipboard('pm2 restart APP_ID_OR_NAME')">📋 Copy</button>

</details>
🛠️ Useful PM2 Commands
<details> <summary>Click to expand commands</summary>
bash
# Stop app
pm2 stop APP_NAME
<button onclick="copyToClipboard('pm2 stop APP_NAME')">📋 Copy</button>

bash
# Delete app from PM2
pm2 delete APP_NAME
<button onclick="copyToClipboard('pm2 delete APP_NAME')">📋 Copy</button>

bash
# Monitor resources
pm2 monit
<button onclick="copyToClipboard('pm2 monit')">📋 Copy</button>

bash
# Reload app (for zero-downtime)
pm2 reload APP_NAME
<button onclick="copyToClipboard('pm2 reload APP_NAME')">📋 Copy</button>

bash
# View specific app info
pm2 show APP_NAME
<button onclick="copyToClipboard('pm2 show APP_NAME')">📋 Copy</button>

</details>

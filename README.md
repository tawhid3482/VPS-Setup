# VPS-Setup

1. System Update & Node.js Installation
# Update package lists
sudo apt update

# Upgrade installed packages
sudo apt upgrade -y

# Install curl
sudo apt install curl -y

# Install Node.js LTS version
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt install -y nodejs

# Verify installation
node -v
npm -v

2. Project Directory Setup
# Create project directory
mkdir -p /var/www
cd /var/www

3. GitHub SSH Configuration

# Check existing SSH keys
ls -al ~/.ssh

# Generate new SSH key (if needed)
ssh-keygen -t ed25519 -C "tawhidulislam3482@gmail.com"

# Start SSH agent
eval "$(ssh-agent -s)"

# Add SSH key to agent
ssh-add ~/.ssh/id_ed25519

# Display public key (copy this to GitHub)
cat ~/.ssh/id_ed25519.pub

# Test GitHub connection
ssh -T git@github.com

4. Clone & Setup Project

# Clone your repository
git clone (git-repo-url)

# List directories
ls

# Enter project folder
cd project-folder

# Install dependencies
npm i

# Build project
npm run build

5. Firewall Configuration

# Update package list
sudo apt update

# Install firewall
sudo apt install ufw -y

# Allow essential ports
sudo ufw allow 22    # SSH
sudo ufw allow 80    # HTTP
sudo ufw allow 443   # HTTPS
sudo ufw allow 3000  # Your project port

# Enable firewall
sudo ufw enable
# Type 'y' when prompted

6. PM2 Process Manager Setup

# Start project (temporary)
npm run start

# Reload firewall
sudo ufw reload

# Install PM2 globally
npm i -g pm2

# Start project with PM2
pm2 start npm --name "project-name" -- start

# Check logs
pm2 logs project-name

# List all PM2 processes
pm2 ls

🔄 Re-deployment Steps (For Updates)
# 1. Pull latest changes
git pull

# 2. Install new dependencies
npm i

# 3. Build project
npm run build

# 4. Check running processes
pm2 ls

# 5. Restart your project (replace <id_no> with your process ID)
pm2 restart <id_no>


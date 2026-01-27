## INSTALLATION

### Browser (No Installation Required)

**Online Editors:**

- Nadesiko3 Storage: https://n3s.nadesi.com/  
- Simple Editor: https://nadesi.com/v3/start

### Node.js (Command Line Version)

**Requirements**: Node.js v18 or higher (recommended)

```bash
# Install globally
npm install -g nadesiko3

# Verify installation
cnako3 --version
```

### From Source (Development)

```bash
# Update system
sudo apt update

# Install Node.js via nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
source ~/.bashrc
nvm install v18.12.1

# Clone nadesiko3
git clone https://github.com/kujirahand/nadesiko3.git
cd nadesiko3
npm install
npm run build

# Optional dependencies
sudo apt install p7zip-full  # For compression commands
sudo apt install xdotool      # For keyboard automation

# Verify
npm test
```

### macOS Additional Tools

```bash
# For compression/extraction commands
brew install p7zip
```

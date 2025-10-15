# 1️⃣ Update system packages
sudo apt update -y

# 2️⃣ Install Apache web server
sudo apt install apache2 -y

# 3️⃣ Enable Apache to start on boot
sudo systemctl enable apache2

# 4️⃣ Start Apache
sudo systemctl start apache2

# 5️⃣ Check Apache status (optional)
sudo systemctl status apache2


# 6️⃣ Go to the default web root directory
cd /var/www/html

# 7️⃣ Remove the default index.html (optional)
sudo rm index.html

# 8️⃣ Upload your website files (replace ‘index.html’ with your actual file)
sudo nano index.html
# or use scp from your local system to upload:
# scp -i your-key.pem index.html ubuntu@<EC2-PUBLIC-IP>:/var/www/html/

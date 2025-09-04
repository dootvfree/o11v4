Installation Guide

Clone the repository:

git clone https://github.com/PrimeHXR/O11-v4
Navigate to the project directory:

cd O11-v4
Install Docker:

snap install docker
Build the Docker image:

sudo docker build -t o11-v4 .
Choose between Node.js or Python. DON'T FORGET TO ADD YOUR SERVER IP ADDRESS!

Remember to update the corresponding file:

server.js: const ipAddress = 'SERVER-IP-HERE';

server.py: IP_ADDRESS = "SERVER-IP-HERE"

Node.js (default):

  sudo docker run -d -p 80:80 -p 443:443 -p 5454:5454 -p 8484:8484 -e IP_ADDRESS=SERVER-IP-HERE -e SERVER_TYPE=nodejs --name o11 o11-v4
Python:

  sudo docker run -d -p 80:80 -p 443:443 -p 5454:5454 -p 8484:8484 -e IP_ADDRESS=SERVER-IP-HERE -e SERVER_TYPE=python --name o11 o11-v4
Access the Web Panel:

URL: http://SERVER-IP-HERE:8484

Credentials: admin:admin

Support the project ❤️
If you liked it, consider donating:

Bitcoin (BTC) Address:
1B6wYR8FJ6sWm8MZSxjT5sdNQtPEHEaykw

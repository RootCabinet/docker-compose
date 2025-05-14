# Simple KALI-Box for quick NMAP
This Docker Compose creates a simple KALI-Box to perform a quick nmap scan. Nothing fancy. 

## Usage
### 1. Build the Docker-Image
```
docker-compose build
```
### 2. Run the Docker Container and connect to a CLI
```
docker-compose run --rm kali-interactive /bin/bash
```

When exiting out of Kali, Container automatically is removed

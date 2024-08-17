# Docker Installation Script for Ubuntu

This repository contains a script to install Docker on Ubuntu systems. Follow the instructions below to clone the repository and run the installation script.

## Cloning the Repository

1. **Clone the Repository**

   Use the following command to clone the repository:

   ```bash
   git clone https://github.com/shegerbootcamp/install-docker-ubuntu.git
   ```

2. **Navigate to the Repository Directory**

   Change into the directory where the script is located:

   ```bash
   cd install-docker-ubuntu
   ```

## Running the Installation Script

1. **Make the Script Executable**

   Ensure that the script has execute permissions:

   ```bash
   chmod +x install_docker.sh
   ```

2. **Run the Script**

   Execute the script to install Docker:

   ```bash
   ./install_docker.sh
   ```

3. **Verify Docker Installation**

   After running the script, you can verify that Docker is installed correctly by checking its version:

   ```bash
   docker --version
   ```

## Adding User to Docker Group

To allow running Docker commands without `sudo`, add your user to the Docker group:

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
```

You may need to log out and log back in for these changes to take effect.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

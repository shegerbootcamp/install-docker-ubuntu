### Instructions on how to run `install_docker.sh`

## Installing Docker

To install Docker on your Ubuntu system, follow these steps:

1. **Download the Installation Script**

   Ensure you have the `install_docker.sh` script available on your local machine. You can download it or copy it to your working directory.

2. **Make the Script Executable**

   Before running the script, you need to make it executable. Open a terminal and run:

   ```bash
   chmod +x install_docker.sh
   ```

3. **Run the Installation Script**

   Execute the script to install Docker:

   ```bash
   ./install_docker.sh
   ```

   The script will:
   - Update the package list and install necessary prerequisites.
   - Add Docker's official GPG key.
   - Add Docker's repository to your APT sources.
   - Install Docker and related packages.
   - Create a Docker group if it doesn’t exist.
   - Add your user to the Docker group.
   - Switch to the Docker group for the current session.

4. **Verify Docker Installation**

   After running the script, you can verify that Docker is installed correctly by running:

   ```bash
   docker --version
   ```

   This command should return the installed Docker version.

5. **Restart Your Terminal Session**

   To apply the group changes, you may need to restart your terminal session. Log out and log back in, or open a new terminal window.

6. **Troubleshooting**

   If you encounter any issues with Docker permissions, ensure that your user is added to the Docker group by checking with:

   ```bash
   groups $USER
   ```

   You should see `docker` listed in the output.

For further Docker usage and configuration details, refer to the [official Docker documentation](https://docs.docker.com/).


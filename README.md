# Linux Pi-hole MOTD

![Pi-hole Logo](https://wp-cdn.pi-hole.net/wp-content/uploads/2023/05/pihole-logo-horizontal-white-e1683321640117.png)

This README provides instructions for setting up a Message of the Day (MOTD) file that displays Pi-hole statistics when you open an SSH session.

## Prerequisites

Before you begin, make sure you have the following:

- A Linux-based system with SSH access
- Pi-hole installed and running on your network

## Installation

1. Connect to your Linux system via SSH.

2. Navigate to the MOTD directory:
    ```bash
    cd /etc/
    ```

3. Create a new MOTD script:
    ```bash
    sudo nano motd
    ```

4. Copy and paste the code from
    ```bash
    PiHole-MOTD
    ```

5. Save and exit the file.

6. Make the script executable:
    ```bash
    sudo chmod +x motd
    ```

7. Test the MOTD script by opening a new SSH session.

## Customization

Feel free to customize the MOTD script to display additional Pi-hole statistics or information. You can modify the existing script or create new scripts in the `/etc/update-motd.d/` directory.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
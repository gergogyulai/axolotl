> New project, might be utterly unusable

# Axolotl

**Axolotl** is a self-hosted, highly configurable Minecraft server manager. It supports multiple server types (Vanilla, Forge, Fabric), different Java versions, mods, resource packs, and more, making it easy to set up and manage advanced Minecraft servers.


## Features

- **Server Types**: Supports Vanilla, Forge, Fabric, and other Minecraft server executables.
- **Java Versions**: Easily switch between different Java versions for compatibility.
- **Mods & Resource Packs**: Add and manage mods, plugins, and resource packs effortlessly.
- **Highly Configurable**: Customize server settings, versions, and features to suit your needs.
- **Dockerized**: Lightweight and portable, runs in a Docker container for easy deployment.


## Installation

### Prerequisites
- Docker installed on your system.
- Basic knowledge of Docker commands.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/axolotl.git
   cd axolotl
   ```

2. Build and run the Docker container:
   ```bash
   docker-compose up -d
   ```

3. Access the Web UI:
   Open your browser and navigate to `http://localhost:8080`.


## Usage

### Starting the Server
- Use the Web UI to start, stop, or restart the server.

### Adding Mods and Resource Packs
- Upload mods and resource packs directly through the Web UI.

### Switching Server Types
- Select Vanilla, Forge, or Fabric from the Web UI and restart the server.

### Configuring Java Versions
- Choose the desired Java version in the settings menu.


## Configuration

### Environment Variables
You can customize the server using the following environment variables:

| Variable              | Description                          | Default Value |
|-----------------------|--------------------------------------|---------------|
| `MINECRAFT_VERSION`   | Minecraft server version to use      | `latest`      |
| `JAVA_VERSION`        | Java version to use                  | `17`          |
| `SERVER_TYPE`         | Server type (Vanilla, Forge, Fabric) | `Vanilla`     |
| `SERVER_PORT`         | Port for the Minecraft server        | `25565`       |

### Docker Volumes
To persist data, mount the following volumes:
- `/data`: Stores server files, mods, and resource packs.

This project is licensed under the [MIT License](LICENSE).

## Support

If you encounter any issues, feel free to open an issue.

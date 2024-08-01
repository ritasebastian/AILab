
```markdown
# Quick Links

- [Ollama](https://ollama.com)
- [Ollama website](https://ollama.com)
- [Ollama Models](https://ollama.com/models)
- [How to install Ollama locally](https://ollama.com/installation)
- [Open WebUI](http://localhost:3000)
- [GitHub Page](https://github.com/open-webui/open-webui)
- [Installation Commands](https://github.com/open-webui/open-webui#installation)
- [Docker Website](https://www.docker.com)
- Localhost URL for OpenWebUI: [http://localhost:3000](http://localhost:3000)

# Setup

To get started, you'll need:

- **Ollama**: an open-source tool for running large language models locally
- **Docker**: software that enables applications to run within containers
- **Open WebUI**: a tool making it simpler to interact with LLMs

# Installation Steps

## Step 1: Install Ollama & Download Models

1. Install Ollama. See prior documentation for details.
2. Proceed to Step 2

## Step 2: Install Docker

1. Visit the [Docker website](https://www.docker.com) and download the application for your operating system (e.g., Mac).
2. Follow installation prompts, accepting the user agreement and using recommended settings.
3. Verify installation by noticing the new Docker icon on your menu bar.

## Step 3: Install Open WebUI in a Docker Container

1. Go to the [Open WebUI repository on GitHub](https://github.com/open-webui/open-webui).
2. Copy the installation command for installing Open WebUI in a Docker container, including dependencies:
   ```sh
   docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
   ```
3. Paste the command into any Terminal application and run it.
4. Verify installation by opening the Docker app and checking that Open WebUI is installed.

## Step 4: Open WebUI Sign-In

1. Navigate to the [Open WebUI URL](http://localhost:3000).
2. Sign up for an admin user account, providing full name, email address, and password.
3. Keep in mind that this information will not be validated or stored externally.

# Adding a New Model

1. Navigate to the model selection in Open WebUI (Top of the page) and search for the desired model (e.g., "Mistral").
2. Type the model name into the search bar and select the option to "pull mistral from ollama.com".
3. The model will be downloaded directly from Ollama.com to your local machine via Ollama.
4. Wait for the download to complete, then check the dropdown menu for the newly added model.
5. Your user must be an administrator for "pull model" to appear!

# Ending and Restarting Open Web UI

1. Close the browser window to exit Open WebUI.
2. To stop using Open WebUI, open the Docker app, locate the container hosting Open WebUI, and click "Stop".
3. If you want to access Open WebUI again, restart the Docker container by clicking the play button.
```

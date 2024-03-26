# Local_LLMs

# Run from an virtualenv
**Create virtualenv:**
- python3 -m virtualenv myenv 
- source myenv/bin/activate 
- jupyter notebook

**Exit virtualenv:**
deactivate


# Open Webui for Ollama

- Option 1: Run with docker-compose
    - `docker-compose up`

- Option 2: Run with docker
    - `docker run -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main`

- Open browser:
    - http://localhost:3000
    - xxxxx
    - xxxxx

- see https://github.com/open-webui/open-webui
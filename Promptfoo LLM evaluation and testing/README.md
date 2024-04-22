# Start

- docker compose up
- Browser: http://localhost:3000

Alternative way via Docker:
- docker build --build-arg NEXT_PUBLIC_PROMPTFOO_BASE_URL=http://localhost:3000 -t promptfoo-ui .
- docker run -p 3000:3000 -v ./local_promptfoo:/root/.promptfoo promptfoo-ui


# Variables in file docker-compose.yml

see https://www.promptfoo.dev/docs/usage/self-hosting

## Examples:

NEXT_PUBLIC_PROMPTFOO_BASE_URL 
tells the web app where to send the API request when the user clicks the 'Share' button. This should be configured to match the URL of your self-hosted instance.

OPENAI_API_KEY
You can also set API credentials on the running Docker instance so that evals can be run on the server. 
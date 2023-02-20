## Chat GPT for discord with openai api

# Setup

1. Copy `.env.example` to `.env` and start filling in the values as detailed below
1. Go to https://beta.openai.com/account/api-keys, create a new API key, and fill in `OPENAI_API_KEY`
1. Create your own Discord application at https://discord.com/developers/applications
1. Go to the Bot tab and click "Add Bot"
    - Click "Reset Token" and fill in `DISCORD_BOT_TOKEN`
    - Disable "Public Bot" unless you want your bot to be visible to everyone
    - Enable "Message Content Intent" under "Privileged Gateway Intents"
1. Go to the OAuth2 tab, copy your "Client ID", and fill in `DISCORD_CLIENT_ID`
1. Copy the ID the server you want to allow your bot to be used in by right clicking the server icon and clicking "Copy ID". Fill in `ALLOWED_SERVER_IDS`. If you want to allow multiple servers, separate the IDs by "," like `server_id_1,server_id_2`
1. Install dependencies and run the bot
    ```
    pip install -r requirements.txt
    python -m src.main
    ```
    You should see an invite URL in the console. Copy and paste it into your browser to add the bot to your server.
    Note: make sure you are using Python 3.9+ (check with python --version)

- Use:

``/chat {message}`` -> create new thread to ask

Restrict: maximum 121 word

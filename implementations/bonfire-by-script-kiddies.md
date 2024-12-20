# Bonfire Project
## Attempted Implementation by team "Script Kiddies"

# What is this Project
A small project that intends to analyse the sentiment of a currently running voice conversation in the Discord chat application and play appropriate background music depending on the mood

# Why did we make this
We wanted to make this in order to create a sense of entertainment and spectacle in something ordinary like a voice conversation.

# How does it work
1. Two users join a voice channel in the Discord chat application
2. The bot detects the presence of the members in the voice channel and joins it
3. The bot recieves the audio stream through the live call
4. This audio stream is transcoded to FLAC format, then analysed by a speech sentiment analysis AI model hosted on the huggingface.co API: https://api-inference.huggingface.co/models/ehcalabres/wav2vec2-lg-xlsr-en-speech-emotion-recognition
5. After analysing the sentiment, the chat bot plays an audio file depending on the sentiment of the current speech

# How to deploy
1. Edit the bot's API key and guild/channel details in `.env` file
2. Run `python src/discordbot.py`

# Why we could not get it working
1. The Discord Voice API does not expose any method to recieve voice streams
2. Various dependency installation errors wasted our development time
3. The latency and time limits of queries to the huggingface.co inference API made the project unusable for testing

# Ideas for fixes
1. Harness Discord gateway/websocket system to recieve and send voice streams
2. Use google colab for access to self-hosted vocal sentiment analysis AI models for low latency
3. Integrate music choice with Spotify/Musicbrainz for advanced sentiment analysis and personalisation

- Contributed by: [Derpitron](https://github.com/Derpitron)
- Contributed by: [RougeDAG](https://github.com/RougeDAG)
- Contributed by: [NandhanaSR](https://github.com/NandhanaSR)

Repo link: https://github.com/Derpitron/breakathon2024-webdev
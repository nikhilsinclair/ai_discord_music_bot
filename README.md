# Discord Bot with GPT-3.5 and Music Playback

## Summary

This Discord bot combines language processing using OpenAI's GPT-3.5 with music playback functionality through YouTube links. The bot interacts with users using a language model and can join voice channels to play music.

## Features

### 1. Chat with AI

The `!talk_ai` command allows users to interact with the bot using natural language. The bot utilizes OpenAI's GPT-3.5 to generate responses. The conversation template is defined in the `template` variable, and the `LLMChain` class handles the interaction.

### 2. Music Playback

Commands like `!play`, `!skip`, `!pause`, `!resume`, and `!stop` control music playback. The bot can connect to voice channels, play YouTube audio, skip tracks, pause, resume, and stop playback. The `YTDLSource` class manages audio playback using the yt-dlp library, and the `play_next` function handles the song queue.

### 3. Greetings

- When the bot connects to the discord server, you are greated with a list of commands explaining how to use the bot.

## Project Structure

- **bot.py:** Main script for running the Discord bot.
- **langchain:** Directory containing language processing functionality.
  - **chains.py:** Defines the `LLMChain` class for managing conversation chains.
  - **llms.py:** Implements the OpenAI language model.
  - **prompts.py:** Provides a template for conversation prompts.
- **yt_dlp:** Library for downloading YouTube videos.
- **ffmpeg:** Executable for audio processing.

## Getting Started (summary)

- To complete this project, I first developed proficiency in both the OpenAI API and Discord API separately. Once I was able to build bots on both of these platforms, I then began integrating the two APIs to make this project.

### Prerequisites

- Python 3.6 or higher
- Discord.py library
- yt-dlp library
- OpenAI GPT-3 API key
- FFmpeg executable

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo

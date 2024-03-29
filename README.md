# VODerino
Automatically launch twitch streams as they go live.

What this application does:

VODerino "listens" to the chat for live notification messages from known chatbots like the streamelements and prismlive chatbots. If one is seen, it will attempt to launch the stream in your set media player. If specified, the application uses the chat's activity based on the number of messages received per minute (or second) to determine if a channel went live.

Setup information:

- This application uses a CLI interface and is intended for use on Windows.
- Unzip the file from the zip package into the same directory.
- Open a command line window and navigate to the directory with the cd command.
- Type VODerino, press enter.
- The guided initial setup will attempt to get required settings, like your Chatterino logs directory. If it's not detected, open Chatterino settings -> Moderation -> Logs tab. Enable logging, then copy the directory and paste it in at the prompt. Note: Chatterino must be open and connected to the chat.

Usage / Syntax:

        VODerino ["Channel_name"] ["Resolution"] ["rec" || "norec"] ["--Permintrig" # || "--Persectrig" #]

        Resolution  -> "audio_only","360p","480p","720p",etc
        rec || norec-> specifies VOD recording or not

        Optional parameters, required for alternate stream detection:

        --Permintrig # -> Launch streams based on the number of messsages seen per minute
        --Persectrig # -> Launch streams based on the number of messsages seen per second
        
REQUIREMENTS
<li class="masthead__menu-item"><a href="https://github.com/streamlink/streamlink">Streamlink</a></li>
<li class="masthead__menu-item"><a href="https://github.com/Chatterino/chatterino2">Chatterino</a></li>

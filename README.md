# VODerino
Automatically open twitch streams when they go live.

WHAT THIS APPLICATION DOES
- VODerino "listens" to the chat for live notification messages from known chatbots like the streamelements and Prismlive chatbots. If one is seen, it will attempt to launch the stream in your set media player. If specified, the application will observe chat movement based on messages received on a minute by minute or second basis to predict if a channel went live.

GENERAL SETUP INFORMATION
- This application uses a CLI interface and is intended for use on Windows.
- Unzip the applications from the zip package. Place the files in the same directory.
- Open a commandline window and navigate to the location you saved the file.
- Type VODerino, press enter.
- The application will attempt to find the required information, such as your Chatterino logs directory in the initial setup menu. If it's not detected, open Chatterino -> Moderation -> Logs tab. Enable logging and copy the directory and paste it in at the required menu prompt. It is assumed required software is installed with their default settings.

HOW TO USE
- Follow the guided initial configuration menu.

USAGE SYNTAX

Usage:
        VODerino ["Channel_name"] ["Resolution"] ["rec" || "norec"] ["--Permintrig" # || "--Persectrig" #]

        Resolution  -> "audio_only","360p","480p","720p",etc
        rec || norec-> specifies VOD recording or not

        Optional parameters, required for alternate stream detection:

        --Permintrig # -> Launch streams based on the number of messsages seen per minute
        --Persectrig # -> Launch streams based on the number of messsages seen per second

REQUIREMENTS
<li class="masthead__menu-item">
          <a href="https://github.com/streamlink/streamlink">Streamlink</a>
        </li>
<li class="masthead__menu-item">
          <a href="https://github.com/Chatterino/chatterino2">Chatterino</a>
        </li>

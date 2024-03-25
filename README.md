# VODerino
Automatically open twitch streams in your favorite media player.

GENERAL SETUP INFORMATION
- Unzip the applications from the zip package. Place the files in the same directory.
- The application will attempt to find the required information, such as your Chatterino directory in the initial setup menu. It is assumed required software is installed with their default settings.

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

# VODerino
If you’re a Twitch viewer who wants to catch streams the moment they go live, VODerino is the tool for you. Unlike other tools that rely on external APIs, it’s designed to monitor Twitch chat activity locally in real-time. As soon as a streamer goes live, VODerino will automatically open the stream in your preferred video or media player, letting you dive straight into the action without a click. There’s also an option to record streams for future viewing.

Whether you want to watch streams live or save them for later viewing, VODerino has you covered.

   ✓ Simple and direct — no API querying or unnecessary complexity.
   
   ✓ Monitors chat activity to detect when a stream goes live.
   
   ✓ Auto-launch streams in your preferred media player.
   
   ✓ Stream recording option to capture and watch later.
   
   ✓ Lightweight and easy to use. Set it and forget it.
    
VODerino – The perfect tool for viewers who want to instantly catch a live stream and have the option to record for later.

Setup Instructions (*This is a Windows CLI application*):

    
    -Unzip the contents of the package into a directory of your choice.
    -Open a Command Prompt window and navigate to the directory using the cd command.
    -Type "VODerino", then press Enter.
    
    The guided initial setup will attempt to retrieve required settings, such as your Chatterino logs directory.
    If it's not automatically detected, open Chatterino and go to Settings → Moderation → Logs tab.
    Enable logging, then copy the log directory path and paste it when prompted.
    
    Note: *Chatterino must be running and connected to the chat for this to work*

Usage / Syntax:

        VODerino ["Channel_name"] ["Resolution"] ["rec" || "norec"] ["--Permintrig" # || "--Persectrig" #]

        Resolution  -> "audio_only","360p","480p","720p",etc
        rec || norec-> specifies VOD recording or not

        Optional Parameters (for more targeted/alternate stream detection):

        --Permintrig # -> Automatically launch the stream based on the number of messages seen per minute.
        --Persectrig # -> Automatically launch the stream based on the number of messages seen per second.
        
REQUIREMENTS
<li class="masthead__menu-item"><a href="https://github.com/streamlink/streamlink">Streamlink</a></li>
<li class="masthead__menu-item"><a href="https://github.com/Chatterino/chatterino2">Chatterino</a></li>

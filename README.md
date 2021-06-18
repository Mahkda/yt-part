# yt-part
Short command line utility to download part of a video available online (might not work on a few websites depending on youtube-dl abilities)

## Options

    -h -help      Show this message   
    -s -start     Where should the download begin (default is 00:00).
                  Format HH:mm:ss.ms (HH: and .ms are optional)
                  or input the number of seconds.number of ms.   
    -l -length    How long the video should be.
                  Format HH:mm:ss.ms (HH: and .ms are optional)
                  or input the number of seconds.number of ms.   
    -n -name      What the output file be named (default is current date)   
    -f -format    Which should the output file be (default is mp4)  
    -vcodec       Which vcodec should the output file be (default is libx264)

## Exemple

If you want to dowload the part of a youtube video between 00:42 and 1:00 and name it output.mp4 you can use :  

`yt-part -start 00:42 -length 00:18 -n output https://www.youtube.com/watch?v=dQw4w9WgXcQ`  

If you want to download the first 30 seconds of a youtube video, and have the output file as a mkv you can use :  

`yt-part -length 30 -format mkv https://www.youtube.com/watch?v=dQw4w9WgXcQ`  

## Licence

This program is released under CC0 licensing, all reutilisation and modification is allowed as long as it keeps this same license
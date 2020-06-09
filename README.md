# tek2mp4
Convert your free tekno music to mp4 video, upload it to YouTube and retrieve the link to share with friends


## OSX

1. Install Homebrew

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

2. Install ffmpeg

`brew install ffmpeg`

3. You must know the location of your audio file on computer
4. You must know where to save the video file made from the audio file on your computer

5. Convert audio to video

`ffmpeg -i /Users/fab/audio_file.aif -filter_complex "[0:a]showwaves=s=1280x720:mode=line:rate=25,format=yuv420p[v]" -map "[v]" -map 0:a /Users/fab/video_file.mp4`

Replace with your own PATH (example: /Users/JohnDoe)

6. Upload the generated video on YouTube

[Listen my track on YouTube ^_^](https://www.youtube.com/watch?v=UI8Too6W-Gk)

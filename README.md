FFmpeg for Nvidia T4 Colab HEVC encoding

I wanted to make a repo for colab's GPU since they can't stay up to date with it and I did it, it took like a week and it was horrible but I did it so you're welcome. If you want to use it, just run these exact commands, if it doesn't work it's cuz you suck, nah tell me if it doesn't work anymore or if the newest version has a feature you want and I'll try to upgrade it.

# Absorb the archive
!wget "https://github.com/AssassinIronMan/FFmpeg/releases/download/v1-no-lib/ffmpeg-nvenc.tar.gz"
# Extract the archive
!tar xzf ffmpeg-nvenc.tar.gz

# Move the executables into /usr/local/bin so they're on your $PATH
!sudo mv ffmpeg-nvenc-release/usr/local/bin/ffmpeg /usr/local/bin/
!sudo mv ffmpeg-nvenc-release/usr/local/bin/ffprobe /usr/local/bin/

# Cleanup
!rm -rf /content/ffmpeg-nvenc-release /content/ffmpeg-nvenc.tar.gz

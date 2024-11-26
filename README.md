# Audio Tools

> Docker-based script for editing audio files

## Dependencies

To be able to use the scripts, the following tools are required:

- Bash
- Docker

## Setup

```sh
cd ~/src/experimental-software
git clone git@github.com:experimental-software/audio-tools.git
cd audio-tools/lib
./build.sh
```

## Usage

### Concatenate MP3 files

```sh
cd /path/to/files
docker run -v $PWD:/home/apprunner/data --rm -it experimentalsoftware/audio-tools /bin/bash
```

```sh
cd ./data
mp3wrap output.mp3 *.mp3
```

**Also see**

- https://askubuntu.com/questions/20507/concatenating-several-mp3-files-into-one-mp3


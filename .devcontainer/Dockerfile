FROM my-pytorch:base

ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=1000

RUN apt update && apt install -y ffmpeg


WORKDIR /pip_installs

COPY whisper.txt .
RUN pip3 install -r whisper.txt

WORKDIR /workspace
USER ${USERNAME}
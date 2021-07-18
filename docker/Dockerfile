FROM alpine:latest

RUN apk update
# RUN apk add curl git wget make libressl-dev libffi-dev ncurses-libs flex bison gperf python3 python3-pip python-future python-cryptography python-pyparsing picocom mc htop nano vim

RUN apk add --no-cache \
	curl \
	wget \
        libressl-dev \
        musl-dev \
	ncurses-libs \
	flex \
	bison \
	python3 \
	python3-pip \
        libffi-dev && \
    pip3 install --no-cache-dir cryptography==2.1.4 && \

# RUN curl http://downloads.whitecatboard.org/console/linux/wcc --output /usr/local/bin/wcc && chmod +x /usr/local/bin/wcc

# USER builder

#RUN cd ~ && wget https://dl.espressif.com/dl/xtensa-esp32-elf-linux64-1.22.0-80-g6c4433a-5.2.0.tar.gz
#RUN mkdir ~/esp && cd ~/esp && tar xzf ~/xtensa-esp32-elf-linux64-1.22.0-80-g6c4433a-5.2.0.tar.gz
#RUN cd ~ && git clone --recursive https://github.com/espressif/esp-idf.git
#RUN /usr/bin/python -m pip install --user -r ~/esp-idf/requirements.txt
#RUN mkdir -p /home/builder/ && cd /home/builder/ && git clone --recursive https://github.com/whitecatboard/Lua-RTOS-ESP32
#ADD build.sh /home/builder/build.sh
#RUN bash /home/builder/build.sh
#ADD .bashrc /home/builder/.bashrc

#USER root

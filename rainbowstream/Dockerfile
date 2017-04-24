FROM python:3.5-alpine

MAINTAINER Felipe Ruhland <felipe.ruhland@gmail.com>

RUN apk --no-cache add \
	build-base \
	freetype \
	freetype-dev \
	libjpeg-turbo-dev \
	openjpeg-dev \
	zlib-dev

RUN pip install --upgrade pip
RUN pip install pillow rainbowstream

ENTRYPOINT [ "rainbowstream" ]

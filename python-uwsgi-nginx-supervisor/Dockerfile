FROM python:3.5-alpine
ENV PYTHONUNBUFFERED 1

RUN apk add --update \
	nginx \
	supervisor \
	openssl \
	postgresql-client \
	postgresql-dev \
	gcc \
	musl-dev \
	linux-headers \
	&& rm -rf /var/cache/apk/*

EXPOSE 8000

CMD ["supervisord", "-n"]

FROM alpine:3.7

# Fill out the labels
LABEL name="handy-alpine" \
      maintainer="Feilong Wang <hustemb@gmail.com>" \
      license="Apache License v2" \
      summary="A handy alpine image supports ssh and python server." \
      version="0.0.1" \
      help="No help" \
      architecture="x86_64" \
      atomic.type="system" \
      distribution-scope="public"

RUN apk add --no-cache ca-certificates python bash openssh-client curl

COPY python_server.py /usr/bin/

EXPOSE 8080

CMD ["python", "/usr/bin/python_server.py"]

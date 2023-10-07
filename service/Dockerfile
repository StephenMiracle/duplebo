FROM golang:1.21 as base


###
# LOCAL DEV
#
FROM base as dev

RUN curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s -- -b $(go env GOPATH)/bin

WORKDIR /opt/app
COPY . /opt/app/
# CMD ["air"]
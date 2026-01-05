FROM golang

WORKDIR /app

COPY . .

# Build the Go app and name the binary 'goapp'
RUN go build -o goapp

# CMD to run the app
CMD ["./goapp"]

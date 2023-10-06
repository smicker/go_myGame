# myGame

A project to test game development in Go, using the Ebitengine lib.

## Requirements
gcc         # Install by `apt install gcc`. Ebitengine also uses C.
some libs   # Install by `sudo apt install libc6-dev libgl1-mesa-dev libxcursor-dev libxi-dev libxinerama-dev libxrandr-dev libxxf86vm-dev libasound2-dev pkg-config`

Environment can be confirmed by the following command:
`go run github.com/hajimehoshi/ebiten/v2/examples/rotate@latest`
which will show a spinning image if everything is installed correctly.

## Run
`go run cmd/main.go`

## Build Linux
`go build cmd/main.go`
or
`GOOS=linux GOARCH=amd64 go build -o myGame cmd/main.go`

## Build Windows
`env GOOS=windows GOARCH=amd64 go build -o myGame.exe cmd/main.go`

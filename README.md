# go-pdfium-render

Experiments using libpdfium shared library in Go for rendering PDF to png.

Mostly taken from: https://github.com/brunsgaard/go-pdfium-render/

## Building/Running on desktop

    PKG_CONFIG_PATH=./ go build main.go
    LD_LIBRARY_PATH=./lib ./main test.pdf

## Cross Compiling

Currently doesn't work

    PKG_CONFIG_PATH=./ GOOS=linux GOARCH=arm GOARM=7 CGO_ENABLED=1 go build main.go 

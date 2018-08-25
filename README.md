# gowasm-example

```sh
GOARCH=wasm GOOS=js go build -o test.wasm main.go

cp $(go env GOROOT)/misc/wasm/wasm_exec.{html,js} .
```

Serve the 3 files and open in broswer.

# Reference
https://github.com/golang/go/wiki/WebAssembly

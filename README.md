# gowasm-example

# Build wasm

The test.wasm was built by `main.go.1` with

```sh
GOARCH=wasm GOOS=js go build -o test.wasm main.go
```

The `wasm_exec.html` and `wasm_exec.js` was copied from Go source code.
```sh
cp $(go env GOROOT)/misc/wasm/wasm_exec.{html,js} .
```

# Build file server

```sh
go get github.com/zyfdegh/gowasm-example

cd $GOPATH/src/github.com/zyfdegh/gowasm-example
```

# Run

```sh
./gowasm-example
```

It serves the 3 wasm files to web. Open http://localhost:8080/wasm_exec.html in broswer
and open the broswer Inspector, then click `Run` and see what's printed in the Console.

# Reference
https://github.com/golang/go/wiki/WebAssembly

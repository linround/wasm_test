# 使用手册
- 初始化项目
```text
go mod init wasm
```
- 安装模块
```text
go mod tidy
```
- 编译wasm
```text
GOOS=js GOARCH=wasm go build -o main.wasm
```
- 生成js
```text
cp "$(go env GOROOT)/misc/wasm/wasm_exec.js" .
```
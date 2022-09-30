# goutils

> 该仓库主要是放置一些开发时积累的代码片段

## 安装

```sh
go get -u github.com/whosydd/goutils
```

## 使用

### `IsExist`: 判断文件或者文件夹是否存在

```go
package main

import (
	"fmt"

	"github.com/whosydd/goutils"
)

func main() {
	dst := "../LICENSE.md"
	flag, err := goutils.IsExist(dst)
	if err != nil {
		fmt.Println(err.Error())
		return
	}
	fmt.Printf("flag: %v\n", flag)
}
```

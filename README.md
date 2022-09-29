# go-utils

## 安装

```sh
go get -u github.com/whosydd/go_utils
```

## 使用

### 判断文件或者文件夹是否存在

```go
package main

import (
	"fmt"

	"github.com/whosydd/go_utils"
)

func main() {
	dst := "../LICENSE.md"
	flag, err := go_utils.IsExist(dst)
	if err != nil {
		fmt.Println(err.Error())
		return
	}
	fmt.Printf("flag: %v\n", flag)
}
```


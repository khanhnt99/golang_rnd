# A Tour of Go
## Packages
- Tất cả các chương trình trong golang đều được tạo thành bởi các packages.
- Programs bắt đầu chạy trong package `main`.
- Program sử dụng các package với import paths `"fmt"` và `"math/rand"`.
- Package name sẽ giống với phần tử cuối cùng của import path. Ví dụ `"math/rand"` package bao gồm các files bắt đầu với statement `package rand`.
- Mục đích của package là design và maintain 1 số lượng lớn các program bằng các nhón các features liên quan lại với nhau thành 1 đơn vị duy nhất -> Dễ dàng maintain, understand, independent of the other package programs. Tính module này cho phép chia sẻ và tái sử dụng. 
- Trong Go, tất cả các packages đều được defined với tên khác nhau và mỗi tên đều gần với chức năng của chúng. Ví dụ như `"strings"` package bao gồm các methods và functions liên quan đến strings.

**Import paths**
- Tất cả các package đều được defined bởi unique string và string này được gọi là `import path` -> Bằng cách sử dụng import path, có thể import packages vào program. `import "fmt"`.

**Package Declaration**
- Package declaration luôn present ở mở đầu của source file và mục đích của package declaration là xác định mã định danh mặc định cho package đó khi được package khác gọi vào. `package main`.

**Import Declaration**
- Import declaration dùng ngay sau package declaration. Go source file bao gồm 0 hoặc nhiều import declaration và mỗi import declaration chỉ định path của nhiều package bên trong dấu `()`.
  ```
  // Import single package
    import "fmt"

  // Import multiple packages
    import (
      "fmt"
      "strings"
      "bytes"
    )
  ```




__Docs__
- https://www.geeksforgeeks.org/packages-in-golang/

__Docs__
- https://go.dev/tour/welcome/1
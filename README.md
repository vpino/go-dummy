Install GO in debian 8


1 — Download Go

````
$ wget https://storage.googleapis.com/golang/go1.8.3.linux-amd64.tar.gz
```

2 — Extract the tarball

```
$ sudo tar -C /usr/local -xzvf 
```

 3 — Setting Go Paths 

 In the file /etc/```profile``` add the following lines:

 ```
export PATH=$PATH:/usr/local/go/bin
 ```

And refres profile

```
$ source /etc/profile
``` 

 4 — Create Workspace

Execute

```
$ mkdir Gospace
```

5 — Add PATH of workspace

In the file /etc/```profile``` add the following lines:

```
export GOPATH=$HOME/Gospace
```

And refresh profile

```
$ source /etc/profile
``` 

6 — Create struct basic that recommend GOLANG 

Execute:

```
$ mkdir -p src/github.com/vpino
```

7 — Create Hello world

```
$ cd $GOPATH/src/github.com/vpino
```

Create directory:

```
$ mkdir hello && cd hello
```

Create the file ```hello.go``` with the following content:

```go
package main

import "fmt"

func main() {
    fmt.Printf("Hello, World!\n")
}
```

8 — Run Hello world

Execute:

```bash
go run hello.go
```

And result:

```bash
Hello, World!
```


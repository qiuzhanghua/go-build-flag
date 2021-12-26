

```bash
 go build -tags debug -ldflags "-X main.version=`autotag current`" -o normal
./normal
```

```bash
go build -tags debug -o debug
./debug
```
output is:

```text
running version is debug
```


```bash
go build -tags release -o release
./release
```
output is:

```text
running version is release
```

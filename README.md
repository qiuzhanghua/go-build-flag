# Learn tags and ldflags for go build

```bash
 go build -tags debug -ldflags "-X main.version=`autotag current`" -o normal
./normal
```
output is:
```text
0.0.1
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

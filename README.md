# go-rpg

The RPG text adventure project from under [raspberrypi.org](https://projects.raspberrypi.org/en/projects/rpg) implemented in Go for educational purposes.

## Development environment

Developed on a [Raspberry Pi 400](https://www.raspberrypi.org/products/raspberry-pi-400/):

```bash
$ uname -a
Linux raspi400 5.8.0-1010-raspi #13-Ubuntu SMP PREEMPT Wed Dec 9 17:14:07 UTC 2020 aarch64 aarch64 aarch64 GNU/Linux
$ go version
go version go1.14.7 linux/arm64
```

## Make

```bash
$ make
usage: make <target>

  where <target> is one of the following

    get         to fetch all dependencies
    build       to compile binary for local machine architecture
    all         to run get, build

    help        to show this text
```

```bash
$ make all
go get github.com/deckarep/golang-set
go build -o rpg
```

## Play

```bash
$ ./rpg 
RPG Game
========

Get to the Garden with a key and a potion
Avoid the monsters!

Commands:
  go "direction"    (where "direction" is one of the following: north, east, south, west)
  get "item"
  exit
---------------------------
You are in the Hall
You see a key
Inventory:
---------------------------
> 
```

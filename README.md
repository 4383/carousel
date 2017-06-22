# Carousel

Carousel is distribued nmap scanner based on dnmap and deployed on docker stack

## usage
```shell
$ git clone https://github.com/4383/carousel
$ cd carousel
$ # edit the nmap scan list to realize
$ vim ./carousel/server/scan.txt # replace by your scan
$ cd carousel
$ docker-compose build
$ docker-compose up
$ # now view your result
$ ls /tmp/dnmap
$ # you can see multiple files corresponding to your scan list
$ # have fun
```

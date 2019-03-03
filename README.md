lua5.1 / Ubuntu (i386) Dockerfile
-
## Includes
1) `i386 Ubuntu 18.04.1 LTS`
2) `lua5.1.5` (https://www.lua.org/)
3) `luarocks`(https://luarocks.org/)

## Get this image

You can execute following command to get this docker image :
```
docker pull ffeast/docker-lua5.1-i386
```


## Purpose
Using `luac` on `x86_64` to produce output working on `i386`


### Example
This is how to produce a i386-compatible lua bytecode file for the sample `test.lua` from this repo:

`docker run -v $(pwd):/lua -it ffeast/lua5.1-i386 luac -o /lua/test.bytecode.lua /lua/test.lua`

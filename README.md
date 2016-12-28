adobe-dng-converter-docker
--------------------------

This image runs Adobe DNG Converter using Ubuntu and WINE.

Instructions
------------

Here's how to convert test.orf into test.dng with full size preview in current directory:
```
docker build -t dng .
docker run --rm -v $(pwd):/work dng -p2 test.orf 
```

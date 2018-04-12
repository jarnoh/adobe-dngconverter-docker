adobe-dngconverter-docker
====

This image runs Adobe DNG Converter using Ubuntu and WINE.  Current version is 10.3.

Instructions
---

Here's how to convert test.orf into test.dng with full size preview in current directory using readymade image from Docker Hub:

```docker run --rm -v $(pwd):/work jarnoh/adobe-dngconverter:latest -p2 test.orf```

To see command-line options, run without parameters:

```docker run --rm -v $(pwd):/work jarnoh/adobe-dngconverter:latest ```

Also see [Command Line Support in the Adobe DNG Converter](http://wwwimages.adobe.com/content/dam/Adobe/en/products/photoshop/pdfs/dng_commandline.pdf)

Building image
---

Clone this repository and build image locally:

```docker build -t jarnoh/adobe-dngconverter .```

Then you can run image as container with:

```docker run --rm -v $(pwd):/work jarnoh/adobe-dngconverter -p2 test.orf ```



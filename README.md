# tinyocr

Recent versions of iOS and macOS offer quite good OCR for images,
which suggested that these systems must now ship with an OCR
library. It turns out they do, so I've made a tiny command line OCR
utility that takes image paths as arguments and emits text to stdout.

This replaces a more elaborate system I've been maintaining for years
with something very minimal. 🥳

## Build

Clone the repo, `cd` into the top level, run:

``` shell
swift build -c release
```

The resulting binary should appear in `./.build/release/tinyocr`. Copy
it to a directory on your path and you should be able to:

``` shell
tinyocr <image>
```

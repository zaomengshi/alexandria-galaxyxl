# alexandria

alexandria is an ebook auto-uploader for various private trackers. It will
fetch metadata for all of your books and upload them if they haven't
been already.

## Installation

Make sure that mktorrent is not lower than 1.1
```
# apt-get install mktorrent poppler-utils djvulibre-bin calibre
$ pip install -r requirements.txt
```

## Usage

```
$ python alexandria /path/to/books
```
The first run will generate an empty config file in ```~/.alexandria/config```
# "Git from the Bottom Up" as ebook

This repository contains the original [Git from the Bottom Up](http://jwiegley.github.io/git-from-the-bottom-up/) converted to EPUB3 and MOBI (KF8:joint) formats.

Credits to the author [John Wiegley](https://github.com/jwiegley).

## DIY

Requirements
- [git](http://git-scm.com/) (not necessary if you download the zip)
- [pandoc](http://pandoc.org/)
- [calibre](http://calibre-ebook.com/)

Instructions:
- Download the original repository (either by git clone or zip download)
```sh
git clone https://github.com/jwiegley/git-from-the-bottom-up
```
- Issue the markdown to epub3 conversion
```sh
pandoc -S -t epub3 -o git-from-the-bottom-up.epub meta.yml index.md 1-Repository/*.md 2-The-Index/*.md \
  	    3-Reset/*.md 4-Stashing-and-the-reflog.md 5-Conclusion.md 6-Further-Reading.md
```
- Use calibre for epub3 to mobi conversion
```sh
ebook-convert "git-from-the-bottom-up.epub" "git-from-the-bottom-up.mobi"
```

## License

The book is from John Wiegley and his contributors at https://github.com/jwiegley. This book is licensed under the [Attribution-NoDerivs](https://creativecommons.org/licenses/by-nd/4.0) license.
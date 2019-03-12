# Bible Reference

A perl script to search for words and lookup verses in the Bible.

*Example Usage*

```
  bible-ref /love/ # find and print all verses containing the string "love" in the Bible
  bible-ref john 3:16 # print the famous Bible verse about God's love
```

Originally by [Martin Ward](http://www.gkc.org.uk/). Hosted on Github with some
modifications by Matthew Thorley.

## Installation

### From source

```
  git clone https://github.com/padwasabimasala/bible-ref.git
  cp bible-ref/bible-ref ~/bin
  mkdir ~/.bibles
  cp bible-ref/KJV ~/.bibles
```

### With Homebrew on Mac

https://github.com/padwasabimasala/homebrew-bible-ref


## Usage

`bible-ref [bible] [book] [chapter:[verse[-verse|,verse]]] {/pattern/in}*`

You can specify any of the bible, book, chapter or a list or range of verse
and/or one or more patterns. The BIBLES environment variable (~/.bibles) gives the
directory where bible versions are stored. The BIBLE variable (KJV) is the name of
the default bible to search.

### Examples:

```
  bible-ref John 3:16         print this famous verse
  bible-ref all John 3:16     print this verse from every available bible
  bible-ref jn 3:             print all of chapter 3 of John's gospel
  bible-ref 3:16              list chapter 3 verse 16 in each book that has one
  bible-ref 3 john            print a whole book
  bible-ref 3 john 2          some books don't have chapter divisions
  bible-ref KJV 1 jn /Jesus/   list verses in 1 John in the KJV which contain Jesus
  bible-ref RSV /Jesus wept/  find the shortest verse in the RSV!
  bible-ref /Adam/ /Eve/      list verses which mention both Adam and Eve
  bible-ref /adam/i           case-insensitive search, finds Adam, adamant etc.
  bible-ref RSV /baalmeon/in  finds the name Ba'al-me'on, ignoring the punctuation
  bible-ref                   print the whole of the default bible
```

Bible etext files formatted for ref available for download from original
author's [website](http://www.gkc.org.uk/martin/software/index.html).

- The Authorised (King James) Version
- The New International Version
- The Revised Standard Version
- The World English Bible (from http://ebible.org)
- The Apocrypha (Revised Standard Version)
- The New Revised Standard Version
- The New American Standard Version
- Young's Literal Translation (1898)
- English Standard Version
- Weymouth New Testament in Modern Speech (1913)

[Original source download](http://www.gkc.org.uk/martin/software/ref)

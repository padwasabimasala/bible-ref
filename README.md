Bible Reference

[Download[(http://www.gkc.org.uk/martin/software/ref)

A perl script to look up Bible references and search for verses.

Usage: ref [bible] [book] [chapter:[verse[-verse|,verse]]] {/pattern/in}*

You can specify any of the bible, book, chapter or a list or range of verse and/or one or more patterns. The BIBLES environment variable gives the directory where bible versions are stored. The BIBLE variable is the name of the default bible to search.

Examples:

  ref John 3:16         print this famous verse
  ref all John 3:16     print this verse from every available bible
  ref jn 3:             print all of chapter 3 of John's gospel
  ref 3:16              list chapter 3 verse 16 in each book that has one
  ref 3 john            print a whole book
  ref 3 john 2          some books don't have chapter divisions
  ref AV 1 jn /Jesus/   list verses in 1 John in the AV which contain Jesus
  ref RSV /Jesus wept/  find the shortest verse in the RSV!
  ref /Adam/ /Eve/      list verses which mention both Adam and Eve
  ref /adam/i           case-insensitive search, finds Adam, adamant etc.
  ref RSV /baalmeon/in  finds the name Ba'al-me'on, ignoring the punctuation
  ref                   print the whole of the default bible

Bible etext files formatted for ref (download and unzip to the BIBLES directory):

The Authorised (King James) Version
The New International Version
The Revised Standard Version
The World English Bible (from http://ebible.org)
The Apocrypha (Revised Standard Version)
The New Revised Standard Version
The New American Standard Version
Young's Literal Translation (1898)
English Standard Version
Weymouth New Testament in Modern Speech (1913)

See http://www.gkc.org.uk/martin/software/index.html for download links.

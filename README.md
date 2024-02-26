# fawf-nyudlts

The FAWF site is a static front-end for NYU-DLTS book viewer.

This repo holds the content, configurations, and child theme for the static pages.

The parent theme is serials-hugo-basetheme.


## Requirements

You need to have Go installed.
  * https://go.dev/doc/install


## Build


###  Build -- all in one

  * rm -rf getremote/markdown/books && hugo -s "getremote" && hugo --cleanDestinationDir

###  Build -- after content is generated

  * hugo --cleanDestinationDir -e _default
  * hugo --cleanDestinationDir -e local
  * hugo --cleanDestinationDir -e stage
  * hugo --cleanDestinationDir -e production

# fawf-nyudlts

The FAWF site is a static front-end for NYU-DLTS book viewer.

This repo holds the 
  * call to remote data source transform content and generate multiple markdown files
  * configurations
  * thumbnail images (TODO: include that in setup process)
  * symlink to parent theme (you should update path)
  *  child theme

The parent theme is serials-hugo-basetheme.


## Requirements

You need to have Go installed.
  * https://go.dev/doc/install

## Setup 

  * Add path to API call in getremote/hugo.toml
  * Add symlink to serials-hugo-basetheme inside of themes directory


## Build


###  Build -- all in one

  * rm -rf getremote/markdown/books && hugo -s "getremote" && hugo --cleanDestinationDir

###  Build -- after content is generated

  * hugo --cleanDestinationDir -e _default
  * hugo --cleanDestinationDir -e local
  * hugo --cleanDestinationDir -e stage
  * hugo --cleanDestinationDir -e production

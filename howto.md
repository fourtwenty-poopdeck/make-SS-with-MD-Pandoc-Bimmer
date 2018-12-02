---
title:
- how to make a slideshow with markdown and pandoc/beamer
theme:
- Copenhagen
---

#setup
+ go to /home/scripts/pandoc/markdown
+ then open up a .md file in your fav text editor

#metadata
i'll just show ex of how to set up metadata:

[three dashes]  
title:  
- how to make slideshows  
author:  
- me  
theme:  
- Copenhagen     
[three dashes]

#basics

+ first off, one hashtag for a heading/ new slide
+ two hashtags for a subsection
+ use + to create an entry in a list

#to change text format:
+ 2 asteriks **bold** 2 asteriks
+ asteric *italic* asteric
+ tilde ~~strikethrough~~ tilde

#add some pics
[exclamation mark][pic caption] file.png

#finally, let's compile and open this bad boy

##compile
pandoc sourcefile.md -t beamer -o outputfile.pdf

##open
mupdf outputfile.pdf

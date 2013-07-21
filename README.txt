sexy-docbooks
=============

Docbook templates that look 'nice'

Good looking docbooks:
---------------------
    - http://hadoopilluminated.com/hadoop_book/index.html
    - http://book.realworldhaskell.org/read/

template 1 : hi-hadoop-book
---------------------------
This template is from 'hadoop illuminated' book (http://hadoopilluminated.com/)

files:
    src/docbks/  <--- where docbook xml files will live
    src/docbks/css  <--- css files
    images   <--- image files

You will need mvn to generate docbooks html
Download maven from http://maven.apache.org/
Once you have maven installed, use the following command to generate docbooks output
    $   mvn  pre-site

to clean and rebuild from scratch
    $   mvn  clean  pre-site

output files are locted here:
    target/site  <--- generated html book (multi page)
    target/site/singlepage  <--- generated html book (single page)

you can just copy the directory 'target/site' to your website.

That is it!  
Now you can start writing your book by editing files in src/docbkx dir

Customizing html output:
    edit file : src/docbk/customization.xsl
    this file includes header / footer sections.

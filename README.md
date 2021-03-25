# ChristianTools
This repository will contain scripts, database files, and many other tools that will help christian software developers.

Bible_Ordered_Chapters.ods and Bible_Ordered_Chapters.xlsx
  The first is an open document spreadsheet to be used for open source spreadsheet software such as libreoffice. The second file (xlsx) is to be used in Microsoft Excel.
   The Column Headers:
      ChronId: This is an integer that represents where the corresponding "(Book,Chapter)" is chronologically
      NormId: This is an integer that represents where the corresponding "(Book,Chapter)" in the normal order of the bible
      Book: This is the book of the bible that the (Book,Chapter) corresponds to.
      Chapter: This is the chapter that the (Book,Chapter) corresponds to.
      Testament: This is the testament (Old Testament or New Testament) that the (Book,Chapter) corresponds to.
      
      
This spreadsheet can be exported to a csv. I have include the .csv file in this directory.

SQLITE3
I have uploaded an sqlite3 database to this repository of these files.
To use this you need to install sqlite3:

Ubuntu/Debian:
  `sudo apt-get update`
  `sudo apt-get install sqlite3`
  
CentOS / Fedora / RedHat:
  `yum install sqlite3`


Some examples of the usage is this:
  `// Get all the bible verses in the old testament in chronological order\n
   SELECT book, verse FROM Bible_Ordered_Chapters WHERE testament="O"`
   

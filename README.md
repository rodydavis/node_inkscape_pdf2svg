## About NODE_INKSCAPE_SVG2PDF
Use Inkscape to convert your PDF images to SVG format. Often times when I download vector files from various sites, it comes in Illustrator AI and EPS formats. What I would do is RENAME the .ai file to .pdf and then use Inkscape to convert the PDF to SVG.
***
## Installation
```
npm install
```
## How to Use

In your terminal console, go to the directory of where you have downloaded these files and run
```
node index.js <path to your PDF file>
```

The SVG will be saved in same directory as your source PDF. You can also specify a directory and it will recursively go through all directories under that target directory and process all SVG files. My samples under PDF directory is set this way. Sample images are from freepik.com where I renamed the .ai files to .pdf so it can be processed by Inkscape.

#### Save results to MySQL Database

The file index_mysql_db.js is for those who want to save the results to MySQL database. I used BookshelfJS library for connecting to MySQL database. In example code, the database name is "media" and the table name is "images".

To process image and save to database, use:

```
node index_mysql_db.js <path to your PDF file>
```


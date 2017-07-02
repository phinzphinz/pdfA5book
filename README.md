# pdfA5book
A bash script that transforms a PDF file such that it can be folded to a DIN A5 book.

## Requirements
- pdftk `sudo apt-get install pdftk`
- pdfjam `sudo apt-get install pdfjam`

## Installation
0.  Make sure that the requirements above are met!
1.  Download the repository `git clone ...`
2.  Make the file `pdfA5book` executable `chmod a+x pdfA5book`
2.  Place the file `pdfA5book` in a directory contained in you $PATH (for example `/bin/`): `sudo cp pdfA5book /bin/`

## Usage 
Say we have a pdf file `raw.pdf` and want to generate the outputfile `out.pdf`, then use the command 
- `pdfA5book raw.pdf out.pdf`

For printing, choose long-bind. Then fold the printed pages appropriately, form a stack and use a tacker.


## Known issues
Sometimes the file size blows up. It may help to use the following commands:

- Convert the output to postscript: `pdf2ps out.pdf out.ps`
- Convert the postscript back to pdf: `ps2pdf out.ps final.pdf`

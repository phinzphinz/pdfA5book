# pdfA5book
_English version below_
## Deutsch
Ein Bash-Skript, das PDF-Dateien transformiert, sodass sie zu einem DIN A5 Buch gefaltet werden können.
_Die folgenden Befehle sind für Ubuntu gültig._
### Voraussetzungen
- pdftk `sudo apt-get install pdftk`
- pdfjam `sudo apt-get install pdfjam`

### Installation
0.  Die Voraussetzungen müssen erfüllt sein!
1.  Das Git-Archiv herunterladen `git clone https://github.com/phinzphinz/pdfA5book.git`
2.  Die Datei `pdfA5book` ausführbar machen: `chmod a+x pdfA5book`
3.  Die Datei `pdfA5book` in ein Verzeichnis der Pfadvariablen ($PATH) hinzufügen (z.B. `/bin/`): `sudo cp pdfA5book /bin/`

### Benutzung
Sei `roh.pdf` die PDF-Datei, die in die Ausgabedatei `ausgabe.pdf` transformiert werden soll. Der dafür auszuführende Befehl lautet 
- `pdfA5book roh.pdf ausgabe.pdf`

Beim Drucken muss Duplexdruck, lange Seite gewählt werden. Dann können die gedruckten Seiten entsprechend gefaltet und zusammengetackert werden.
### Bekannte Probleme
Manchmal steigt die Dateigröße durch die Transformation drastisch an. In diesem Fall können die folgenden Befehle Abhilfe schaffen:
- Die Datei `ausgabe.pdf` in Postscript umwandeln: `ps2pdf ausgabe.pdf ausgabe.ps`
- Die Postscriptdatei zurück in PDF umwandeln: `ps2pdf ausgabe.ps enddatei.pdf`

### Spenden
BTC: 1MPdFPdnor1mDTUtXTZVG5PJnzQgcKmmwG

---
## English
A bash script that transforms a PDF file such that it can be folded to a DIN A5 book.
_The following commands are valid for Ubuntu._

### Requirements
- pdftk `sudo apt-get install pdftk`
- pdfjam `sudo apt-get install pdfjam`

### Installation
0.  Make sure that the requirements above are met!
1.  Download the repository `git clone https://github.com/phinzphinz/pdfA5book.git`
2.  Make the file `pdfA5book` executable: `chmod a+x pdfA5book`
3.  Place the file `pdfA5book` in a directory contained in you $PATH (for example `/bin/`): `sudo cp pdfA5book /bin/`

### Usage 
Say we have a pdf file `raw.pdf` and want to generate the outputfile `out.pdf`, then use the command 
- `pdfA5book raw.pdf out.pdf`

For printing, choose duplex long-bind. Then fold the printed pages appropriately, form a stack and use a tacker.


### Known issues
Sometimes the file size blows up. It may help to use the following commands:

- Convert the output to postscript: `pdf2ps out.pdf out.ps`
- Convert the postscript back to pdf: `ps2pdf out.ps final.pdf`

### Donate
BTC: 1MPdFPdnor1mDTUtXTZVG5PJnzQgcKmmwG

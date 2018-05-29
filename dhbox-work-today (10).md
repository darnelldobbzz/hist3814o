    1  ls
    2  cd ocr-test
    3  sudo apt-get install tesseract-ocr
    4  sudo apt-get install imagemagick
    5  convert -density 300 ~/war-diary/e001518087.jpg -depth 8 -strip -background white -alpha off e001518087.tiff
    6  tesseract e001518087.tiff output.txt
    7  sudo apt-get update
    8  sudo apt-get install libcurl4-gnutls-dev
    9  sudo apt-get install libmagick++-dev
   10  sudo apt-get install libtesseract-dev
   11  sudo apt-get install libleptonica-dev
   12  sudo apt-get install tesseract-ocr-eng
   13  sudo apt-get install libpoppler-cpp-dev
   14  history 
   15  history > dhbox-work-today.md

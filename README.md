# Introducción a p5.js
Repository for the source material for the Spanish translation of Getting Started with p5.js. The book is now available on [processingfoundation.press](https://processingfoundation.press/). A physical copy of the book can be ordered [here](https://www.amazon.com/Introducci%C3%B3n-p5-js-Spanish-Lauren-McCarthy/dp/0999881302).

## Production
The following contains documentation for setting up the project locally in order to generate PDF builds for upcoming versions and changes.

### Getting Started
First, clone this repository with the following using terminal:
```bash
git clone https://github.com/processing/p5.js-getting-started-es.git
```
As we will be using [magicbook](https://github.com/magicbookproject/magicbook) for this project, make sure to install the `magicbook` package:
```bash
npm install magicbook -g
```
### Fonts
In order to make a proper build, you will need to have the correct typefaces in the `fonts/` folder which are listed in `fonts/font-list.txt`.

### Making a Build
To make a new build, first make sure you are in the project folder.
```bash
cd p5.js-getting-started-es
magicbook build
```

### Editing the Book
To make changes to the book, locate the necessary files in `content/` and use a text editor of your choice. Likewise, any updates to the images can be made using the editing software of your choice on files from the `images/` folder. The stylesheet which contains all of the styling for the book is `stylesheets/pdf.scss`.

Should you need to edit which files are included in the build, open `magicbook.json` with your text editor.


### PDF vs Printed
**IMPORTANT:** Depending on what type of build you are making (printed or digital), make sure to update the last two digits of the ISBN in `content/copyright.html`. The PDF ISBN is designated for the PDF distributed online at [processingfoundation.press](https://processingfoundation.press/) while the PRINT ISBN is designated for the physical copy.

Use a PDF editor/converter such a Adobe Acrobat Pro to attach the correct cover and title page files – as these will also be build-specific. The respective PDF files can be found in `cover/`. All builds must have a title page; if you are creating a physical copy, the full cover will be submitted separately along with an interior-only PDF build.

You may also want to remove the folio on the last two pages (p228-229).

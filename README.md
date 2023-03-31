# TCPDF Library for Joomla!

__If you already know how to use TCPDF and you need it for a Joomla! project, than this is a library package to be used in Joomla! Easy to install and update.__

TCPDF is a PHP class for generating PDF files on-the-fly without requiring external extensions.
This library includes also a class to extract data from existing PDF documents and classes to generate 1D and 2D barcodes in various formats.

## Main Features:
* no external libraries are required for the basic functions;
* all standard page formats, custom page formats, custom margins and units of measure;
* UTF-8 Unicode and Right-To-Left languages;
* TrueTypeUnicode, OpenTypeUnicode v1, TrueType, OpenType v1, Type1 and CID-0 fonts;
* font subsetting;
* methods to publish some XHTML + CSS code, Javascript and Forms;
* images, graphic (geometric figures) and transformation methods;
* supports JPEG, PNG and SVG images natively, all images supported by GD (GD, GD2, GD2PART, GIF, JPEG, PNG, BMP, XBM, XPM) and all images supported via ImagMagick (http://www.imagemagick.org/script/formats.php)
* 1D and 2D barcodes: CODE 39, ANSI MH10.8M-1983, USD-3, 3 of 9, CODE 93, USS-93, Standard 2 of 5, Interleaved 2 of 5, CODE 128 A/B/C, 2 and 5 Digits UPC-Based Extension, EAN 8, EAN 13, UPC-A, UPC-E, MSI, POSTNET, PLANET, RMS4CC (Royal Mail 4-state Customer Code), CBC (Customer Bar Code), KIX (Klant index - Customer index), Intelligent Mail Barcode, Onecode, USPS-B-3200, CODABAR, CODE 11, PHARMACODE, PHARMACODE TWO-TRACKS, Datamatrix, QR-Code, PDF417;
* JPEG and PNG ICC profiles, Grayscale, RGB, CMYK, Spot Colors and Transparencies;
* automatic page header and footer management;
* document encryption up to 256 bit and digital signature certifications;
* transactions to UNDO commands;
* PDF annotations, including links, text and file attachments;
* text rendering modes (fill, stroke and clipping);
* multiple columns mode;
* no-write page regions;
* bookmarks, named destinations and table of content;
* text hyphenation;
* text stretching and spacing (tracking);
* automatic page break, line break and text alignments including justification;
* automatic page numbering and page groups;
* move and delete pages;
* page compression (requires php-zlib extension);
* XOBject Templates;
* Layers and object visibility.
* PDF/A-1b support.

### Third party fonts:

This library may include third party font files released with different licenses.

All the PHP files on the fonts directory are subject to the general TCPDF license (GNU-LGPLv3),
they do not contain any binary data but just a description of the general properties of a particular font.
These files can be also generated on the fly using the font utilities and TCPDF methods.

All the original binary TTF font files have been renamed for compatibility with TCPDF and compressed using the gzcompress PHP function that uses the ZLIB data format (.z files).

The binary files (.z) that begins with the prefix "free" have been extracted from the GNU FreeFont collection (GNU-GPLv3).
The binary files (.z) that begins with the prefix "pdfa" have been derived from the GNU FreeFont, so they are subject to the same license.
For the details of Copyright, License and other information, please check the files inside the directory fonts/freefont-20120503
Link : http://www.gnu.org/software/freefont/

The binary files (.z) that begins with the prefix "dejavu" have been extracted from the DejaVu fonts 2.33 (Bitstream) collection.
For the details of Copyright, License and other information, please check the files inside the directory fonts/dejavu-fonts-ttf-2.33
Link : http://dejavu-fonts.org

The binary files (.z) that begins with the prefix "ae" have been extracted from the Arabeyes.org collection (GNU-GPLv2).
Link : http://projects.arabeyes.org/

### ICC profile:

TCPDF includes the sRGB.icc profile from the icc-profiles-free Debian package:
https://packages.debian.org/source/stable/icc-profiles-free

* **category**    Library
* **author**      Nicola Asuni <info@tecnick.com>
* **copyright**   2002-2022 Nicola Asuni - Tecnick.com LTD
* **license**     http://www.gnu.org/copyleft/lesser.html GNU-LGPL v3 (see LICENSE.TXT)
* **link**        http://www.tcpdf.org
* **source**      https://github.com/tecnickcom/TCPDF

## Developer(s) Contact

* Nicola Asuni <info@tecnick.com>

> Compiled into an installer for Joomla 3 by [Llewellyn van der Merwe](mailto:joomla@vdm.io) at [Vast Development Method](https://www.vdm.io/)

# Usage in Joomla (PHP)
```php
// Import TCPDF library
jimport('tcpdf.tcpdf');
```
or
```php
// Import TCPDF library
require_once JPATH_LIBRARIES . '/tcpdf/tcpdf.php';
```
Now you can create a new PDF document:
```php
$pdf = new TCPDF();
```

# Documentation
+ [Source Code Documentation](http://www.tcpdf.org)
+ [Additional Documentation](http://www.tcpdf.org)

# Automatic updates
This library is integrated with Joomla's automatic updates. Before updating it's mandatory that you check that your documents still work as expected.

# License
TCPDF is licensed under LGPL ([GNU LESSER GENERAL PUBLIC LICENSE](https://github.com/vdm-io/tcpdf/blob/master/LICENSE.TXT))

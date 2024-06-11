This fork is archived
=====================

This fork existed for pre-release use of https://github.com/xperseguers/t3ext-extractor/commit/93e9db04fe3bfbafb9fbf8a650bdc247ef425977, which has since made it into the upstream `causal/extractor` package.

Thus, this fork is now archived. Please switch to the upstream package.

Metadata and content analysis service
=====================================

This extension detects and extracts metadata (EXIF / IPTC / XMP / ...) from
potentially thousand different file types (such as MS Word/Powerpoint/Excel
documents, PDF and images) and bring them automatically and natively to TYPO3
when uploading assets. Works with built-in PHP functions but takes advantage of
Apache Tika and other external tools for enhanced metadata extraction.

.. image:: Documentation/Images/metadata.png
   :alt: Metadata for a document


Requirements
------------

For best results, `Apache Tika <https://tika.apache.org/download.html>`__ is
required (either as standalone JAR or running as server).

Extraction of metadata from common image files (jpg, tiff, ...) is often quicker
using external tool `exiftool <https://exiftool.org/>`__ and if not available,
it will fall back to PHP's built-in EXIF and IPTC library.

For PDF, external tool
`pdfinfo <https://www.xpdfreader.com/pdfinfo-man.html>`__ will be used.


Read more in the
`manual <https://docs.typo3.org/p/causal/extractor/master/en-us/>`__.

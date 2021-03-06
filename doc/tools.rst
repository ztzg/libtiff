TIFF Tools Overview
===================

.. image:: images/quad.jpg
    :width: 144
    :alt: quad

This software distribution comes with a small collection of
programs for converting non-TIFF format images to TIFF and for
manipulating and interrogating the contents of TIFF images. Several
of these tools are useful in their own right. Many of them however
are more intended to serve as programming examples for using the
TIFF library.

Device-dependent Programs
-------------------------

There are two device-dependent programs that serve as simple
examples for writing programs to display and save TIFF images.

.. list-table:: Device-dependent programs
    :widths: 5 20
    :header-rows: 1

    * - Tool
      - Description

    * - `tiffgt <man/tiffgt.1.html>`_
      - Display the contents of one or more TIFF images using OpenGL.
        The software makes extensive use of the ``TIFFRGBAImage``
        facilities described elsewhere.

Device-independent Programs
---------------------------

The remaining programs should be device-independent:

.. list-table:: Device-dependent programs
    :widths: 5 20
    :header-rows: 1

    * - Tool
      - Description

    * - `fax2ps <man/fax2ps.1.html>`_
      - Convert a Group 3- or Group 4- compressed TIFF to PostScript
        that is significantly more compressed than is generated by
        :program:`tiff2ps` (unless :program:`tiff2ps` writes PS Level II)

    * - `fax2tiff <man/fax2tiff.1.html>`_
      - Convert raw Group 3 or Group 4 facsimile data to TIFF

    * - `pal2rgb <man/pal2rgb.1.html>`_
      - Convert a Palette-style image to a full color RGB image by
        applying the colormap

    * - `ppm2tiff <man/ppm2tiff.1.html>`_
      - A quick hack that converts 8-bit PPM format images to TIFF

    * - `raw2tiff <man/raw2tiff.1.html>`_
      - Create a TIFF file from raw data

    * - `rgb2ycbcr <man/rgb2ycbcr.1.html>`_
      - Convert an RGB, grayscale, or bilevel TIFF image to a YCbCr
        TIFF image; it's mainly provided for testing

    * - `thumbnail <man/thumbnail.1.html>`_
      - Copy a bilevel TIFF to one that includes 8-bit greyscale
        "thumbnail images" for each page; it is provided as an example of
        how one might use the ``SubIFD`` tag (and the library support
        for it)

    * - `tiff2bw <man/tiff2bw.1.html>`_
      - A simple program to convert a color image to grayscale 

    * - `tiff2pdf <man/tiff2pdf.1.html>`_
      - Convert TIFF images to PDF

    * - `tiff2ps <man/tiff2ps.1.html>`_
      - Convert TIFF images to PostScript

    * - `tiff2rgba <man/tiff2rgba.1.html>`_
      - Convert a TIFF image to RGBA color space

    * - `tiffcmp <man/tiffcmp.1.html>`_
      - Compare the contents of two TIFF files (it does not check all
        the directory information, but does check all the data)

    * - `tiffcp <man/tiffcp.1.html>`_
      - Copy, concatenate, and convert TIFF images (e.g. switching from
        ``Compression=5`` to ``Compression=1``) 

    * - `tiffcrop <man/tiffcrop.1.html>`_
      - Provides selection of images from within one or more multi-image
        TIFF files, with orthogonal rotation, mirroring, cropping, and
        extraction of multiple sections and exporting to one or more files.
        It extends the functionality of :program:`tiffcp` to support additional bit
        depths in strips and tiles and enhances the selection capabilities of
        tiffsplit. Bilevel images can be inverted and images may be split into
        segments to fit on multiple /pages/ (standard paper sizes), plus other
        functions described in the tiffcrop man page 

    * - `tiffdither <man/tiffdither.1.html>`_
      - Dither a b&w image into a bilevel image (suitable for use
        in creating fax files)

    * - `tiffdump <man/tiffdump.1.html>`_
      - Display the verbatim contents of the TIFF directory in a file
        (it's very useful for debugging bogus files that you may get from
        someone that claims they support TIFF)

    * - `tiffinfo <man/tiffinfo.1.html>`_
      - Display information about one or more TIFF files

    * - `tiffmedian <man/tiffmedian.1.html>`_
      - A version of Paul Heckbert's median cut program that reads an
        RGB TIFF image, and creates a TIFF palette file as a result

    * - `tiffset <man/tiffset.1.html>`_
      - Set a field in a TIFF header

    * - `tiffsplit <man/tiffsplit.1.html>`_
      - Create one or more single-image files from a (possibly)
        multi-image file

Check out the manual pages for details about the above programs.

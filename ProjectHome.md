Ever since the as3 corelib from Adobe was released, developers got some good tools to encode and export an image from Flash using into various formats.

But Adobe only included some popular image file formats, sometimes you just need more.

This class let's you encode to a  ["portable graymap format"](http://en.wikipedia.org/wiki/Netpbm_format).image (.pgm).

It works just the same as the as3corelib image encoders from adobe.

1) copy the PGMEncoder.as into the as3corelib images folder (com\adobe\images)

2) to use the class inside your project its just like the jpg or png encoders:

> PGMEncoder.encode(bmd);

where bmd stands for your bitmapdata object.
# pgm-exporter
Automatically exported from code.google.com/p/pgm-exporter

#How to use the encoder

How to use the class
usage:
It works just the same as the as3corelib image encoders from adobe.

1) copy the PGMEncoder.as into the as3corelib images folder (com\adobe\images)

2) to use the class inside your project its just like the jpg or png encoders:

PGMEncoder.encode(bmd);
where bmd stands for your bitmapdata object.

example:

function takePicture(){
    counter++;
    bmd.draw(video);
    var ba:ByteArray = PGMEncoder.encode(bmd);

    var file:File = File.desktopDirectory.resolvePath("imageName" + counter + ".pgm");
    var fileStream:FileStream = new FileStream();
    fileStream.open(file, FileMode.WRITE);
    fileStream.writeBytes(ba);
    fileStream.close();
}

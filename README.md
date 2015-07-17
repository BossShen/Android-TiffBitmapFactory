# Android-TiffBitmapFactory
TiffBitmapFactory is an Android library that allow open *.tif image files on Android devices.

Just now it has possibility to open tif image as mutable bitmap, read count of directory in file, apply sample rate for bitmap decoding.

# Usage
Read directory count of image:
TiffBitmapFactory.getDirectoryCount(String path_to_file)

Open file: 
TiffBitmapFactory.decodePath(String path_to_file)
TiffBitmapFactory.decodeFile(File file)

Additional usage:
TiffBitmapFactory class contains inner class Options that allow to tune some parameters
Options.inJustDecodeBounds - if set to true will return blank bitmap with width, height and decode config
Options.inSampleSize - set sample size for decoding. if sample size > 1 than image will be reduced
Options.directoryCount - set directory to read from image
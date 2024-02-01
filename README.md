PHP Image Toolbox (GB Lib)
=============
Based on Image_Toolbox by Martin Theimer https://sourceforge.net/projects/image-toolbox/  

Main functions:

1. Convert to JPEG  
2. Make thumbnail  
3. Make thumbnail box  
4. Make thumbnails with aspect ratio  
5. Image cropping  
6. Blend watermarks

Examples
--------

<b>Upload as JPEG</b>

```php
$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
$img->save( '/tmp/destination.file', 'jpg'); 
```

<b>Make thumb</b>
```php
$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
$img->newOutputSize( 100, 100, 4 );  
$img->save( '/tmp/destination.file' ); 
```

<b>Make thumb (aspect ratio)</b>
```php
$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
$img->newOutputSize( 100, 0, 4 );  
$img->save( '/tmp/destination.file' ); 
```

<b>Make thumb (merge center)</b>
```php
$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
$img->newOutputSize( 100, 0, 1 );  
$img->save( '/tmp/destination.file' ); 
```

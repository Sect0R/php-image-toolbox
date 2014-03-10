PHP Image Toolbox
=============

Main functuins:

1. Convert to JPEG  
2. Make thumbnail  
3. Make thumbnail box  
4. Make thumbnails with aspect ratio  
5. Image cropping  
6. Blend watermarks

Examples
--------

<b>Upload as JPEG</b>


	$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
	$img->save( '/tmp/destination.file', 'jpg'); 



<b>Make thumb</b>

	$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
	$img->newOutputSize( 100, 100, 4 );  
	$img->save( '/tmp/destination.file' ); 


<b>Make thumb (aspect ratio)</b>

	$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
	$img->newOutputSize( 100, 0, 4 );  
	$img->save( '/tmp/destination.file' ); 

<b>Make thumb (merge center)</b>

	$img = new Image_Toolbox( $_FILES['file']['tmp_name'] );  
	$img->newOutputSize( 100, 0, 1 );  
	$img->save( '/tmp/destination.file' ); 

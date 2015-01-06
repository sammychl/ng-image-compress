ng-image-compress
=================

######This Angular directive compresses jpeg or png files using angularjs on client side. It uses using HTML5 Canvas &amp; File API. The compression algorithm is based off of the J-I-C project on github. 
###### There's an old angularjs-imageupload-directive from mischi package that claims to do image compress, but somehow it doesn't compress images nearly as well as the J-I-C project's. Thus, this repo here. Some of the code was borrowed from the above too, so u will find similarities. Note: I have absolutely no clue why J-I-C's compression is better.
-----------

Steps:

  1. add ng-image-compress.js directive as a dependency in your index.html
  2. add ng-image-compress tag to ur html `<input type="file">` elements. 
  
Example for you to fiddle a bit below (u might want to upload the image after compression thus the `ng-file-select="onFileSelect($files)`. To do this, you'll first need to `bower install ng-file-upload`):

`<input id="inputImage" type="file" accept="image/*" ng-image-compress="image2" resize-max-height="1000" resize-max-width="1000" resize-quality="0.7" resize-type="image/jpg" ng-file-select="onFileSelect($files)" />`

**These can be adjusted: resize-max-height, resize-max-width, resize-quality, resize-type 

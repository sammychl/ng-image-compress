ng-image-compress
=================

######This Angular directive compresses jpeg or png files using angularjs on client side. It uses using HTML5 Canvas &amp; File API. The compression algorithm is based off of the J-I-C project on github. 
###### There's an old angularjs-imageupload-directive from mischi package that claims to do image compress, but somehow it doesn't compress images nearly as well as the J-I-C project's. Thus, this repo here. Some of the code was borrowed from the above too, so u will find similarities. Note: I have absolutely no clue why J-I-C's compression is better.
-----------

Steps:

  1. bower install ng-image-compress then add ng-image-compress.js directive as a dependency in your index.html
  2. add image tag to ur html <input> element. eg. image="myAwesomeImage"
  3. add <img ng-src="{{myAwesomeImage.compressed.dataURL}}"> to ur html page to see the compressed photo.
  4. do whatever u want to do with the compressed file. eg. use angular-file-upload package to upload it.
  
Example:

`<input id="inputImage" type="file" accept="image/*" image="image1" resize-max-height="1000" resize-max-width="1000" resize-quality="0.7" resize-type="image/jpg" />`

**Adjustable: resize-max-height, resize-max-width, resize-quality, resize-type 


For demo, u can just clone this repo and then run index.html. thanks!!
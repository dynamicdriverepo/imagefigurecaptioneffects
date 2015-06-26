# Image Figure Caption effects #

*Description:* Images may tell a thousand words, but with a nice caption it can tell a few more. This script transforms any image into a HTML5 compliant figure element with a nice caption. It also works on existing figure elements. Choose from 7 different effects to unveil the caption in style. Captions can be dynamically defined or literally inside the figure element. For captions that exceed the height of the image, scrollbars are added to make the hidden portion accessible.

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.113 or above (served via Google CDN)
+ TweenMax.min.js (served via CDN)
+ figurecaptions.css
+ figurecaptions.js

*Step 2:* Add the below code to the HEAD section of your page:

	<link rel="stylesheet" href="figurecaptions.css" />
	
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
	<script src="http://cdnjs.cloudflare.com/ajax/libs/gsap/latest/TweenMax.min.js"></script>
	
	
	<script src="figurecaptions.js">
	
	/***********************************************
	* Image Figure Caption effects- (c) Dynamic Drive DHTML code library (www.dynamicdrive.com)
	* This notice MUST stay intact for legal use
	* Visit Dynamic Drive at http://www.dynamicdrive.com/ for this script and 100s more
	***********************************************/
	
	</script>
	
	<script>
	
	$(function(){ // on DOM load
		$('#eg1').addCaption({ // very long caption
			caption: '<p>An awesome picture caption!</p><p>An awesome picture caption!</p><p>An awesome picture caption!</p><p>An awesome picture caption!</p><p>An awesome picture caption!</p>'
		})
	
		$('#eg2').addCaption({ // dynamic caption
			fx: 'zoomin',
			caption: 'An awesome picture caption!'
		})
	
		$('#eg3').addCaption({
			fx: 'dualpanels',
			caption: 'An awesome picture caption!'
		})
	
		$('#eg4').addCaption({ // caption from container's "title" attribute
			fx: 'dualpanels2',
			caption: 'title'
		})
	
		$('#eg5').addCaption({
			fx: 'pushup',
			caption: 'title'
		})
	
		$('#eg6').addCaption({ // caption from figure element's figcaption element
			fx: 'flipopen'
		})
	
		$('#eg7').addCaption({
			fx: 'flipreveal'
		})
	
	})
	
	</script>

*Step 3:* Add the below to the BODY section of your page

	<img id="eg1" src="sunbreakthrough.jpg" /> 
	
	<img id="eg2" src="sunbreakthrough.jpg" />
	
	<img id="eg3" src="sunbreakthrough.jpg" />
	
	<img id="eg4" src="sunbreakthrough.jpg" title="An awesome picture caption!" />
	
	<img id="eg5" src="sunbreakthrough.jpg" title="An awesome picture caption!"/>
	
	<figure id="eg6">
		<img src="sunbreakthrough.jpg" alt="An awesome picture">	
		<figcaption>An awesome picture caption! <a href="http://www.dynamicdrive.com">A link</a></figcaption>
	</figure>
	
	<figure id="eg7">
		<img src="sunbreakthrough.jpg" alt="An awesome picture">	
		<figcaption>An awesome picture caption! <a href="http://www.dynamicdrive.com">A link</a></figcaption>
	</figure>


## Image Figure Caption effects ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex15/imagefigurecaption.htm>

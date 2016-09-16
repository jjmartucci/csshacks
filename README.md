# csshacks
Collection of CSS hacks with use cases.

## Hide play button on iOS videos

    video::-webkit-media-controls-start-playback-button {
		  display: none !important;
	  }
	  
## Hide select arrow in IE

    select::-ms-expand {
  	  display: none;
    }
    
## Change color of link on tap
    -webkit-tap-highlight-color: red

    
## Sub-pixel font smoothing [source](https://www.mobomo.com/2014/5/better-font-smoothing-in-chrome-on-mac-os-x/)

    html {-webkit-font-smoothing: antialiased; } 

    @media only screen and (-webkit-min-device-pixel-ratio: 1.25), only screen and ( min-device-pixel-ratio: 1.25), only screen and ( min-resolution: 200dpi), only screen and ( min-resolution: 1.25dppx) {
      -webkit-font-smoothing: subpixel-antialiased; 
    } 

## iOS Momentum Scrolling
     -webkit-overflow-scrolling: touch

## Break at newline characters
Useful when using a plain text field to series of items.

	white-space: pre-line;

## Break inline text at every word
Useful if you want text wrapped in a span to break to a new line at every word.

	.parent {
		width: 200px;
	}
	
	.child {
		word-spacing: 200px; // for fluid layouts, you can use something like 9999999px
	}

## Prevent User Select and User Drag.
Not prefixed by autoprefixer as it's not standard.

	-webkit-user-select: none;
  	-moz-user-select: none;
  	-ms-user-select: none;
  	user-select: none;
  	-webkit-user-drag: none;
  	user-drag: none;

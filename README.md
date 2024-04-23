# pricing-tiers
The code and description of a mock front-end trial pricing page.

This page was built in my website design certification course. 

For this code, I worked on creating a responsive page with columns and buttons that change on hover. I used stock pictures and descriptions to stay true to the design, along with the suggestive button to point to the price tier I would like the consumer to purchase. For this page, I used color contrast theory to find the best light blue color to show against the white of the different tiers. The words are bold and are in a font that is easy to read. The letters are spaced enough to know what each one is, however, the words are a little too small and the greyish-blue color is a little too bright so it's not showing off the white. 

**HTML CODE**
I chose not to use alt text for the images because they are purely decorative. The message of the webpage is conveyed without the description of the images.


<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Price Tiers</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:400,600,700">
    <link rel="stylesheet" href="app.css">
</head>

<body>
    <div class="panel">

        <div class="pricing-plan">
            <img src="icons/icon1.png" alt="" class="pricing-img">
            <h2 class="pricing-header">Personal</h2>
            <ul class="pricing-features">
                <li class="pricing-features-item">Custom domains</li>
                <li class="pricing-features-item">Sleeps after 30 mins of inactivity</li>
            </ul>
            <span class="pricing-price">Free</span>
            <a href="#/" class="pricing-button">Sign up</a>
        </div>

        <div class="pricing-plan">
            <img src="icons/icon2.png" alt="" class="pricing-img">
            <h2 class="pricing-header">Small team</h2>
            <ul class="pricing-features">
                <li class="pricing-features-item">Never sleeps</li>
                <li class="pricing-features-item">Multiple workers for more powerful apps</li>
            </ul>
            <span class="pricing-price">$150</span>
            <a href="#/" class="pricing-button is-featured">Free trial</a>
        </div>

        <div class="pricing-plan">
            <img src="icons/icon3.png" alt="" class="pricing-img">
            <h2 class="pricing-header">Enterprise</h2>
            <ul class="pricing-features">
                <li class="pricing-features-item">Dedicated</li>
                <li class="pricing-features-item">Simple horizontal scalability</li>
            </ul>
            <span class="pricing-price">$400</span>
            <a href="#/" class="pricing-button">Free trial</a>
        </div>

    </div>

</body>

</html> 


**Original CSS Code:**

	/* http://meyerweb.com/eric/tools/css/reset/ 
  	 v2.0 | 20110126
   	License: none (public domain)
	*/

	html, body, div, span, applet, object, iframe,
	h1, h2, h3, h4, h5, h6, p, blockquote, pre,
	a, abbr, acronym, address, big, cite, code,
	del, dfn, em, img, ins, kbd, q, s, samp,
	small, strike, strong, sub, sup, tt, var,
	b, u, i, center,
	dl, dt, dd, ol, ul, li,
	fieldset, form, label, legend,
	table, caption, tbody, tfoot, thead, tr, th, td,
	article, aside, canvas, details, embed, 
	figure, figcaption, footer, header, group, 
	menu, nav, output, ruby, section, summary,
	time, mark, audio, video {
		margin: 0;
		padding: 0;
		border: 0;
		font-size: 100%;
		font: inherit;
		vertical-align: baseline;
	}
 
	/* HTML5 display-role reset for older browsers */
	article, aside, details, figcaption, figure, 
	footer, header, hgroup, menu, nav, section {
		display: block;
	}
 
	body {
		line-height: 1;
	}
 
	ol, ul {
		list-style: none;
	}
 
	blockquote, q {
		quotes: none;
	}
 
	blockquote:before, blockquote:after,
	q:before, q:after {
		content: '';
		content: none;
	}
 
	table {
		border-collapse: collapse;
		border-spacing: 0;
	}

	html {
	  	box-sizing: border-box;
	  	font-family: 'Open Sans', sans-serif;
	}
	
	body {
 		background-color: #60a9ff;
  		display: flex;
 	 	justify-content: center;
 	 	align-items: center;
  		min-height: 100vh;
	}

	.panel {
 	 	background-color: white;
 	 	border-radius: 10px;
  		**padding: 15px 25px;**
  		width: 100%;
  		max-width: 960px;
  		display: flex;
  		flex-direction: column;
  		text-align: center;
  		text-transform: uppercase;
	}

	.pricing-plan {
  		**border-bottom: 1px solid #e1f1ff;**
	}
 
	.pricing-plan:last-child {
 	 	border-bottom: none;
	}

	.pricing-img {
		**margin-bottom: 25px;**
  		**max-width: 100%;**
	}

	.pricing-header {
 	 	**color: #888;**
 		font-weight: 600;
 		letter-spacing: 1px;
	}

	.pricing-features {
 	 	**margin: 50px 0 25px;**
  		color: #016ff9;
	}

	.pricing-features-item {
	  	**font-weight: 600;**
	  	letter-spacing: 1px;
	  	**font-size: 12px;**
 	 	line-height: 1.5;
 	 	padding: 15px 0;
 	 	**border-top: 1px solid #e1f1ff;**
	}

	.pricing-features-item:last-child{
  	   	**border-bottom: 1px solid #e1f1ff;**
	}

	.pricing-price {
	    	**color: #016ff9;** 
  	   	display: block;
  	    	font-size: 32px;
	   	font-weight: 700;
	}

	.pricing-button {
 	    	border: 1px solid #9dd1ff;
	 	border-radius: 10px;
 	   	**color: #348efe;**
            	display: inline-block;
	   	padding: 15px 35px;
 	    	text-decoration: none;
	    	margin: 25px 0;
	    	transition: background-color 200ms ease-in-out;
	}

	.pricing-button:hover, .pricing-button:focus {
	    	**background-color: #e1f1ff;**
	}

	.pricing-button.is-featured {
 	 	**background-color: #48aaff;**
	  	color: white;
	}

	.pricing-button.is-featured:hover, .pricing-button.is-featured:focus{
	 	**background-color: #269aff;**
 	  	color: white;
	}


	@media (min-width: 900px){
	    .panel {
  	      	flex-direction: row;
	    }
 	    .pricing-plan {
 	      	border-bottom: none;
 	      	**border-right: 1px solid #e1f1ff;**
	      	padding: 25px 50px;
	   }
	  .pricing-plan:last-child {
 	     	border-right: none;
	  }
	}

**Accessible CSS Code:**

	/* http://meyerweb.com/eric/tools/css/reset/ 
	   v2.0 | 20110126
	   License: none (public domain)
	*/

	html, body, div, span, applet, object, iframe,
	h1, h2, h3, h4, h5, h6, p, blockquote, pre,
	a, abbr, acronym, address, big, cite, code,
	del, dfn, em, img, ins, kbd, q, s, samp,
	small, strike, strong, sub, sup, tt, var,
	b, u, i, center,
	dl, dt, dd, ol, ul, li,
	fieldset, form, label, legend,
	table, caption, tbody, tfoot, thead, tr, th, td,
	article, aside, canvas, details, embed, 
	figure, figcaption, footer, header, group, 
	menu, nav, output, ruby, section, summary,
	time, mark, audio, video {
		margin: 0;
		padding: 0;
		border: 0;
		font-size: 100%;
		font: inherit;
		vertical-align: baseline;
	}
	
 	/* HTML5 display-role reset for older browsers */
	article, aside, details, figcaption, figure, 
	footer, header, hgroup, menu, nav, section {
		display: block;
	}
	body {
		line-height: 1;
	}
	ol, ul {
		list-style: none;
	}
	blockquote, q {
		quotes: none;
	}
	blockquote:before, blockquote:after,
	q:before, q:after {
		content: '';
		content: none;
	}
	table {
		border-collapse: collapse;
		border-spacing: 0;
	}

	html {
  		box-sizing: border-box;
  		font-family: 'Open Sans', sans-serif;
	}

	body {
	  	background-color: #60a9ff;
	 	display: flex;
 		justify-content: center;
 	 	align-items: center;
		min-height: 100vh;
	}

	.panel {
 		background-color: white;
  		border-radius: 10px;
 		**padding: 25px 25px;**
  		width: 100%;
  		max-width: 960px;
 	 	display: flex;
 	 	flex-direction: column;
 	 	text-align: center;
  		text-transform: uppercase;
	}

	.pricing-plan {
  		**border-bottom: 1px solid #53708a;**
	}
	
 	.pricing-plan:last-child {
  		border-bottom: none;
	}

	.pricing-img {
		**margin-bottom: 12px;**
 		**max-width: 110%;**
	}

	.pricing-header {
  		**color: #5f5f5f;**
  		font-weight: 600;
  		letter-spacing: 1px;
	}

	.pricing-features {
 		**margin: 50px 0 50px;**
 		color: #016ff9;
	}

	.pricing-features-item {
  		**font-weight: 675;**
 		letter-spacing: 1px;
  		**font-size: 14px;**
  		line-height: 1.5;
  		padding: 15px 0;
  		**border-top: 1px solid #7797b3;**
	}

	.pricing-features-item:last-child{
		**border-bottom: 1px solid #7797b3;**
	}

	.pricing-price {
		**color: #0062da;** 
  		display: block;
  		font-size: 32px;
  		font-weight: 700;
	}

	.pricing-button {
  		border: 1px solid #9dd1ff;
  		border-radius: 10px;
  		**color: #2d7ad8;**
  		display: inline-block;
  		padding: 15px 35px;
  		text-decoration: none;
  		margin: 25px 0;
  		transition: background-color 200ms ease-in-out;
	}

	.pricing-button:hover, .pricing-button:focus {
  		**background-color: #cce5fc;**
	}

	.pricing-button.is-featured {
  		**background-color: #3d8cd1;**
  		color: white;
	}

	.pricing-button.is-featured:hover, .pricing-button.is-featured:focus{
  		**background-color: #0062da;**
  		color: white;
	}


	@media (min-width: 900px){
  		.panel {
    			flex-direction: row;
  		}
 		.pricing-plan {
   			border-bottom: none;
   			**border-right: 1px solid #7797b3;**
    			padding: 25px 50px;
  		}
  		.pricing-plan:last-child {
   			border-right: none;
		}
	}	

By changing the colors, font weight and size, margins, and padding, I was able to make the words more readable and easily seen no matter the size of your screen. 

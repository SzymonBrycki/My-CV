# My CV

## A CV / Resume template of a webpage.

This is how to use the repo if you wanna put your own information in there.

# CSS

## Colors

To change the default colors, go to **style.css** file in CSS folder. Find the part below:

```
:root
{
	/* background color */
	--bcolor: #F1F1E6;
	
	/* front color */
	--fcolor: #191970;
	
	/*new front color: #191970 */
	/*old front color: #3D486B */
	
	/* th (table header) color */
	--thcolor: #B9D9EB;
	
	/*new th color: #4B9CD3 */
	/*old th color: #C5CEC2 */
}
```

This part defines the color palette used by default. Background color [**bcolor**] definies the color of non-text (white in pure HTML with no CSS), front color [**fcolor**] the color of text. Additionally, there's a table header color [**thcolor**] that definies the color of headers of tables. You can change them in this section however you wish.

# HTML

You will mostly wanna edit this part. Go to template folder and find **index.html**.

## Name header

The first section you will edit is probably gonna be this one. You can just edit the right parts in index.html file. For those of you who are interested: this should be in two divs, like that:

```
<div class="myheader">
	<div class="myheader2">
		Name and surname
	</div>
</div>
```

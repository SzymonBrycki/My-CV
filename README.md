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

## Auto-div

All of the below divs should be in one big, big div of **class "auto-div"**.
 
## Name header

The first section you will edit is probably gonna be this one. You can just edit the right parts in index.html file. For those of you who are interested: this should be in two divs, like that:

```
<div class="myheader">
	<div class="myheader2">
		Name and surname
	</div>
</div>
```

## Basic info

The next div should be of **class "basic-info**". You can put there whatever you wanna - your LinkedIn and social media, place of residence, phone number, email address itp.

## Personal statement

The next div should be of **class "career-goals**". You can put your personal statement in here.

## Class container

The next part is kinda tricky, This is the place where the CV gets divided into 2, non-equal parts (right and left or main and additional). You should create a big div of **class "container"**. 

Inside this div, there should be two more, one of **class "divs-equal"** and **id "main-part"**. The second should be also of **class "divs-equal"** and have the **id "additional-part"** 

Inside **every** single one of the divs shoul be yet another one, with **class "div-padding"**.

### Main part

This div is meant to showcast your most inportant info, such as work experience and education. When describing them, use the following scheme:

```
<div class="table-job">
	<div class="table-job-job">Job <br>
		<span class="span-date">20XX - 20XX</span></div> 
	<div class="table-job-middle">-</div> 
	<div class="table-job-description">description</div>
</div>
```

For education do the very same, just change "job" into "degree" or "diploma".

Of course, the above should get filled with actual titles, jobs, educational achievements, years of and description. 

For description, I would suggest to fill it with place (per instance "Ney Your City, USA") and maybe additional details about university or school ("Oregon State University"). Because there is not too much of space, they should get separated with `<br>` (this also looks nice).

[You can also put within main part other things you are particularly proud of and want to catch the attention of a recruiter.]

#### Dates

Dates are set within a span of **class "span-date"**. They should be in the same div as job/educational achievement, just separated with `<br>` - again, because of space issues and looks.

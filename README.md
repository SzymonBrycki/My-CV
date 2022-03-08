# My CV

## A CV / Resume template of a webpage.

This is how to use the repo if you wanna put your own information in there.

# Some initial info

You need basically the contents of `IMG`, `CSS` and `Template` folders. `My-own-CV` can be deleted if you download this from GitHub, as it contains my personal information based on the same website tmeplate..

`Template` contains the ready-to-be-filled scheme of the website. Refer to README only if you find that you cannot fill it correctly or something feels confusing to you.

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

### Additional part

Below is the description of elements that can go into div of **id "additional-part**.

#### Languages

This CV project contains a special table and elements made specially with foreign languages in mind. 

##### Languages table

The table structure for languages look as below:

```
<table class="center-table no-space">

	<tr>
		<th class="center-inside-table"><b>Language</b></th>
		<th class="center-inside-table"><b>CEFR Level</b></th>
		<th class="center-inside-table"><b>Certification</b></th>
	</tr>
	
	<tr>
		<td class="center-inside-table"><b><span class="language-info" title="Number of known words 1">Language 1</span></b></td>
		<td><b>Native</b> language</td>
		<td> </td>
	</tr>
	
	<tr>
		<td class="center-inside-table"><b><span class="language-info" title="Number of known words 2">Language 2</span></b></td>
		<td><b>B2</b></td>
		<td><b>Certificate 1</b></td>
	</tr>
	
	<tr>
		<td class="center-inside-table"><b><span class="language-info" title="Number of known words 3">Language 3</span></b></td>
		<td><b>A2</b></td>
		<td><b>Certificate 2</b> </td>
	</tr>
</table>
```
Now, the description, if this all looks somehow enigmatic:

Table header elements (th) should be of class **"center-inside-table"**, so should be td elements containing the name of a language.

Name of a language should be within span of **class "language-info"**. It should also have argument **title with value describing how many words in a given language you know**. After moving your mouse over the elements (which will be underlines with dots) curson will change and the title will be printed. 

###### Advice on languages

I strongy advice you to use CERF levels when talking about your foreign languages, and also use the scheme above to give details about your certification in a given language. At minimum, you should use **title** within **language-info span** to provide additional information to your recruiter. 

#### Skills

There is also a second table, meant for skills. The basic code looks like below:

```
<table class="center-table">
								
	<tr>
		<td colspan="2" class="table-center-text"><b>Broad group 1</b></td>
	</tr>
								
	<tr>
		<td><b>Skill 1</b></td>
		<td>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-black">★</span>
			<span class="star-black">★</span>
		</td>
	</tr>
								
	<tr>
		<td><br></td>
	</tr>
								
	<tr>
		<td colspan="2" class="table-center-text"><b>Broad group 2</b></td>
	</tr>
								
	<tr>
		<td><b>Skill 2</b></td>
		<td>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-black">★</span>
			<span class="star-black">★</span>
		</td>
	</tr>
								
	<tr>
		<td><b>Skill 3</b></td>
		
		<td>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-black">★</span>
		</td>
	</tr>
								
	<tr>
		<td><br></td>
	</tr>
								
	<tr>
		<td colspan="2" class="table-center-text"><b>Broad group 3</b></td>
	</tr>
								
	<tr>
		<td><b>Skill 4</b></td>
		<td>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-gold">★</span>
			<span class="star-black">★</span>
		</td>
	</tr>
								
</table>
```
Description and explanation to make it all less criptic below:

Broad group of skills ("programming languages", "databases", "management skills" etc.) should be set to **colspan=2** and be of **class "table-center-text"**.

Skills should be inside a `<td>` with their name. Then a second `<td>` should follow, with 5 spans of class either **star-gold** or **star-black** with every span containing one black star in UTF (★). This will color them accordingly, to gold or black color. This way is very simple to show how good you are at various skills.

If you wanna separate various skill group with a "space", you can add the below code after the last skill in a skill group:
```
<tr>
	<td><br></td>
</tr>
```

## Divs at the end

### Break

Before the copyright section, you should enter an empty div with **class "break"**.

### Copyrights

The last div you should put in your website is this:
```
<div class="copyrights">
	<p>Copyright © 2020 - <script> data = new Date(); document.write(data.getFullYear());</script> Szymon Brycki
	<br>
	<a href="https://github.com/SzymonBrycki/My-CV">GNU GPL version 3 or later.</a>
	<br>				
	Some rights reserved. </p>
</div>
```

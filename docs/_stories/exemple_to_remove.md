---
layout: default
category: description 
title: Exemple part 
id: 1 
---
<!--- category : Enter the category here in description, correlation, prediction. You can create new ones in '_config.yml' -->
<!--- title : Set the name to the precise part -->
<!--- id : The id is just to set the order of the parts inside a category -->




<!--- The title set above is already a level 2 title so use only title with 3# or more -->
### Title level 3  


<!--- Description here -->
Hello darkness my old friend...  
<!--- Becareful, you have to put 2 spaces '  ' in order to break the line -->
You're beautiful, my friend   

<!--- Between one star '*' in italic, two for bold -->
*italic* and **bold**
[Markdown Guide](https://www.markdownguide.org/cheat-sheet/)
[Markdown Cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)


<!--- If you want to do something more advanced use HTML -->
<!--- Warning, you can use Markdown inside HTML tags -->
<center> My centered text !</center>  
Let focus on HTLM **tags**  
[HTML GUIDE](https://htmlcheatsheet.com/)  
[HTML CHEATSHEET](https://web.stanford.edu/group/csp/cs21/htmlcheatsheet.pdf)  

<!--- Puce list -->
My list :
- element
- element
- another element

<!--- Manual Line Break -->
<br />
<br />
<br />

<center> <h3>centered title level 3 </h3> </center>  
<center> <h4>centered title level 4 </h4></center>  
<center> <h5>centered title level 5 </h5> </center>  

<br />
<br />
<br />

#### Reference to a plot
<p align="center">
<img src="img/plots/correlation_expenses_roads.png" alt="My Image" height="75%" width="75%">
<br />
<i>Exemple for a legend</i>
</p>
<br />
<br />
<br />

#### Reference to a beautifulplot
<p align="center">
<iframe src="img/plotly/correlation_expenses_roads.html" height="600" width="100%"></iframe>
<br />
<i>Exemple for a legend</i>
</p>
<br />
<br />


#### Reference to a dataframe  

<p align="center">

<iframe src="img/dataframes/proportion_permis.html" height="300" width="100%"></iframe>
</p>
<br />
<br />

#### Reference to a dataframe nice

<p align="center">

<iframe src="img/dataframesly/proportion_permis.html" height="300" width="100%"></iframe>
</p>
<br />
<br />

#### Reference to a maps

<p align="center">
<iframe src="img/maps/accident_canton.html" height="600" width="100%"></iframe>
<br />
<i>Exemple for a legend</i>
</p>

<br />
<br />
<br /> 

### WOW TWO ELEMENTS

<div class="row">
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/plotly/correlation_expenses_roads.html" height="600" width="100%"></iframe>
    </div>
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/maps/accident_canton.html" height="600" width="100%"></iframe>
    </div>

</div>
<br /> 
<br /> 


### WOW TWO WITH DIFFERENTES PROPORTIONS

<!--- The size of a column is defined by the number after col-md-* the sum has to be 12 -->
[Bootstrap principle](https://www.w3schools.com/bootstrap/bootstrap_grid_system.asp)  
[Exemples](https://www.w3schools.com/bootstrap/bootstrap_grid_examples.asp)

<div class="row">
    <div class="col-xs-12 col-md-9">
    	<iframe src="img/plotly/correlation_expenses_roads.html" height="600" width="100%"></iframe>
    </div>
    <div class="col-xs-12 col-md-3">
    	<iframe src="img/maps/accident_canton.html" height="600" width="100%"></iframe>
    </div>

</div>

<br /> 
<br /> 

### WOW TWO WITH DIFFERENTES PROPORTIONS AND VERTICAL CENTER

<div class="row">
	<div style='height:600px;' class="col-xs-12 col-md-3"> <!--- don't forget to set the set height as above -->
		<div  class="vertical-center"> <!--- to center vertical -->
			<blockquote> My amazing text center is the middle of the block! </blockquote>
			<i> Oh yeah! I like this guy </i>
		</div>
    </div>
    <div style='height:600px;' class="col-xs-12 col-md-9">
    	<iframe src="img/plotly/correlation_expenses_roads.html" height="100%" width="100%"></iframe>
    </div>
    

</div>
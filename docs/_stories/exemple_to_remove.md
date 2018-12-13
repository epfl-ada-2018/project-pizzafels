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
<img src="img/plots/accident_2months.png" alt="My Image" height="75%" width="75%">
<br />
<i>Exemple for a legend</i>
</p>
<br />
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

#### Reference to a dataframe
<p align="center">
{% include_relative dataframes/proportion_permis.html %}
</p>
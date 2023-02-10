# Web Track learning project
## Meet-up 1  Nav-Bar  ---- To see Preview press **Crtl + V** ----

Hyper Text Markup Language (**HTML**)  and Cascading Style Sheet (**CSS**)

**Friday Feb 3rd 2023** \
We learn about the basic structure of HTML

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta http-equiv="X-UA-Compatible" content="IE=edge" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Navbar</title>
		<link rel="stylesheet" href="styles.css" />
	</head>
	<body>
		<header>
			<h1>Name</h1>
			<nav>
				<ul>
					<a href="index.html"><li>Home</li></a>
					<a href="about.html"><li>About</li></a>
					<a href="contact.html"><li>Contact</li></a>
					<a href="carrers.html"><li>careers</li></a>
				</ul>
			</nav>
		</header>

		<main>
			<h3>This is our home page</h3>
		</main>
	</body>
</html>

```
We also did some basic styling
```css
* {
	padding: 0;
	margin: 0;
	font-family: Verdana, Geneva, Tahoma, sans-serif;
}

/* Navbar styles */

header{
	display: flex;
	flex-direction: row;
	align-items: center;
	justify-content:space-between;
	padding-right: 20px;
	padding-left: 20px;
	box-shadow: 5px 5px 10px rgb(241, 241, 241);
	background-color: rgb(247, 247, 247);
}

header h1{
	text-transform: uppercase;
	cursor: pointer;
}

ul {
	display: flex;
	gap: 20px;
	justify-content: end;
	list-style: none;
}

li {
	padding: 15px;
	color: black;
}

li:hover {
	background-color: seagreen;
}

ul a{
	text-decoration: none;
}

ul a:hover{
	text-decoration: underline;
}

/* Main tag styles */
main{
	margin-top: 20px;
	margin-left: 10px;
}

main h3{
	color: crimson;
}
```
### Some concepts learned were
* The vsCode shortcut which gives you a starter boilerplate code. This can be achieved by typing an exclamation **!** then pressing **Enter** 
*  The declaration is used to tell the browser what version of HTML is used. `` <!DOCTYPE html> ``
* **HTML** tag is the root of the document i.e it encloses everything as seen from above.
*  To link out stylesheet we would place this in our head tag. `` <link rel="stylesheet" href="name.css" /> ``
* **Element nesting** where we can have an element inside another element. e.g The **div** having a **p** in it.
 ```html
    <div>
		<p>Home</p>
	</div>
```
* **CSS Selectors** which are used to select elements when styling them in our css files.
   * class selector   `` <p class="my-class"> This is my text </p> ``
   * id selector `` <p  id="my-id"> This is my text </p> ``
* We also saw we can select an element in CSS using its tag 
   ```css
   header{
	display: flex;
	flex-direction: row;
	align-items: center;
	justify-content:space-between;
	padding-right: 20px;
	padding-left: 20px;
	box-shadow: 5px 5px 10px rgb(241, 241, 241);
	background-color: rgb(247, 247, 247);
	}
     ```
* **CSS specificity** This is used to select a specific element by giving some sort of a path to it e.g
  ```css
  header h1{
	text-transform: uppercase;
	cursor: pointer;
	}
  ```
  Here we tell our css we want to style a **h1** element inside our **header** element.

* **CSS Flexbox**
    * **Flexbox** is a CSS box model that allows you to create a flexible layout.
    * It can be achieved by changing the **display** property of our container.
    * After making a container a **flex-box** we can now use some new properties **flex-direction**,  
      **justify-content** and **align-items**.
     This in turn makes out container a flexible box.
	 	* **flex-direction:row;** or **:column** dictates the direction of the elements are placed a row  
	 	  or a column 
		* **justify-content:space-between;** adds space between the elements
		*  **align-items:center;** makes sure all items are in the center of the flex-box vertically
	 ```css
	header{
	display: flex;
	flex-direction: row;
	justify-content:space-between;
	align-items: center;
	}
	 ```

### This is what we were able to come-up with.
![Nav-bar](images/navbar.png)

&nbsp;  
&nbsp;  

<hr>

<div style="display:flex;flex-direction:column;align-items:center;">
    <h3>Speakers</h3>
    <p>Cliff Omollo <a href="https://github.com/OsegoTech">GitHub</a></p>
    <p>Abel Misiocha <a href="https://github.com/Codedwells">GitHub</a></p>
</div>
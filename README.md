# Personal Portoflio
## It is a simple portfolio website using HTML and CSS and hosted on github
### It is for learning purpose but will keep improving it
### Some website features :-
* Sementic HTML for SEO Purposes
* Responsive CSS to work on all screens
* Used Google Poppins font
* Some animations when hovering over elements
## Website Link 
* Here is the link for the website: https://abdelrahmanbaher4.github.io/personal_portoflio/
## Website Demo :
### Website Navigation :- 
![Alt Text](https://media.giphy.com/media/aInxCCl06erdi1y2I0/giphy.gif)
#### 1) Header
* made it fixed by setting value of position to fixed
* gave z-index a high value to make it the only thing appearing while scrolling
```css
header{
    background-color: #f0f0f0;
    width: 100%; 
    /*it will make the header fixed when scrolling*/
    position: fixed;
    z-index: 999;/*high value make it the only thing appearing when scrolling*/
    display: flex;  
    justify-content: space-between;
    align-items: center;
    padding: 10px 200px; /* top&bottom , right&left*/
}
```
* for the logo and navigation used em in font-size to be a relative font-size where each 1em=16px 
* hovering over any element in the navigation bar turns the element to purple
 ```css
.logo{
     text-decoration: none; /* will remove the line for hre*/
     color: #3a6cf3;  
     text-transform: uppercase;  
     font-weight: 700;
     font-size: 1.8em; /* em relative to what is defined in the body & browser default 16px */
}
.navigation a {
    color: #3a6cf3;
    text-decoration: none;
    font-size: 1.1em;
    font-weight: 400;
    padding-left: 30px;
}
.navigation a:hover {
   color: purple; 
}

```
#### 2) Education 
* made a shadow for the card 


### Making the website responsive 
* tried to make it for all kind of screens handling three main widths
** less than 1023px , less than 641px , less than 300px
```css

@media (max-width:1023px){
    header{
        padding: 12px 20px;
    }
    .navigation{
        padding-left: 10px;
    }
    .title{
        font-size: 1.8em;
    }
    section{
        padding: 80px 20px;
    }
    .main h2{
        font-size: 1em;
    }
    .main h3{
        font-size: 1.6em;
    }
    .content{
        flex-direction: column;
        align-items: center ;
    }
}

@media (max-width:641px){
    body{
        font-size: 12px;
    }
    .main h2{
        font-size: 0.8em;
    }
}
@media (max-width:300px){
    body{
        /*1 em = 10px*/
        font-size: 10px;
    }
    .main h2{
        font-size: 0.8em;
    }
}



```








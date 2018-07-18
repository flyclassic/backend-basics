# digital-dips

### For other coding references, and examples: 
* HTML - https://www.w3schools.com/html/default.asp
* CSS - https://www.w3schools.com/css/default.asp
* JS - https://www.w3schools.com/js/default.asp

### Useful tools
* Image uploader: https://imgbb.com/upload
* Online Code Editor : http://codepen.io

# Exercise 1
```html
<html>
    <header>
      <title>My First HTML page</title>
    </header>
    <body>
        <h1>My first heading</h1>
        <p>My first paragraph</p>
    </body>
</html>

```


# Exercise 2 
#### https://codepen.io/wil-fu/pen/vjWqdp

### Assets URL

* Mickey sprite - https://image.ibb.co/jxZ7uJ/sprite2.png

### HTML

```html
<html>
<header>
  <title>Oh No!</title>
</header>

<body>
  <h1>Example 2</h1>
  <p>Oh No!</p>
  <div class="sprite"></div>
</body>

</html>
```
### CSS
```css
h1,
p {
  font-family: Avenir;
  text-align: center;
}

.sprite {
  width: 320px;
  height: 240px;
/*   border: 1px solid #000; */
  display: block;
  background: transparent
    url(https://image.ibb.co/jxZ7uJ/sprite2.png)
    0 0 no-repeat;
  margin: 20px auto;
  animation: walker 2s steps(12) infinite;
}


@keyframes walker {
  from {
    background-position: 0 0;
  }
  to {
    background-position: 0 -2880px;
  }
}



```


# Exercise 3 
#### https://codepen.io/wil-fu/pen/RBNmOy

### Assets URL

* Background image - https://image.ibb.co/mYQLkT/bg_main.jpg
* Placements Ads image - https://image.ibb.co/hhKJ1y/placement_ad.jpg
* Link Destination - https://www3.lenovo.com/ph/en/jedichallenges/

### Video Embed Code

```html <iframe class="embed-trailer" src="https://secure.disney.com/embed/567d0efa99233716e22d0479?domain=video.disney.ph" frameborder="0" allowfullscreen=""></iframe>```

### HTML

```html
<html>

<head>
  <title>Example 3</title>
</head>

<body>
  <h1>Example 3</h1>
  <p><button>Shop Now</button></p>

   <a class="placement-ad" href="https://www3.lenovo.com/ph/en/jedichallenges/"><img src="https://image.ibb.co/hhKJ1y/placement_ad.jpg" /></a>
 
  <iframe class="embed-trailer" src="https://secure.disney.com/embed/567d0efa99233716e22d0479?domain=video.disney.ph" allowfullscreen=""></iframe>

</body>

</html>
```

### CSS

```css
h1,
p {
  font-family: Avenir;
  text-align: center;
  color:#fff;
}

body{ 
  background-image:url(https://image.ibb.co/mYQLkT/bg_main.jpg);
  background-position:top;
  background-size:cover;
  background-repeat: no-repeat;
}

button {
  background-color: #4caf50;
  border: none;
  color: white;
  padding: 20px 20px;
  font-size: 20px;
}


button:hover {
  color: black;
  background-color: #CCCCCC; /* light grey */
  cursor: pointer;
}

.placement-ad{
  display: block; /* A block-level element starts on a new line and stretches out to the left and right as far as it can. */
  margin: auto auto; /* center the block */
  padding: 10px;
  width: 960px;
  border: 2px solid #fff;
  background:#fff;
}

.embed-trailer{
  border: none;
  display: block; /* A block-level element starts on a new line and stretches out to the left and right as far as it can. */
  margin: auto auto;
  width: 900px;
  height: 510px;
}
```
### Javascript
```javascript
$("button,.placement-ad").click(function(){
  $(".placement-ad").toggle('slow');
});
```


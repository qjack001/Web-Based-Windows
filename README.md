<h1 align="center">
  <br>
  <a href="https://qjack001.github.io/Web-Based-Windows/"><img src="https://raw.githubusercontent.com/qjack001/Web-Based-Windows/master/assets/computer.png" alt="Computer Logo" width="80"></a>
  <br>
  <a href="https://qjack001.github.io/Web-Based-Windows/">Web Based Windows</a>
</h1>

<h4 align="center"><a href="https://qjack001.github.io/Web-Based-Windows/">Web-Based-Windows</a> is a stupid website that imitates the look and feel of early Windows operating systems.<br>It was created to experiment with draggable and resizable divs, as well as <a href="http://brutalistwebsites.com/">brutalist website design</a>.</h4>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How to Use</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#credits">Credits</a> •
  <a href="#authors">Authors</a> •
  <a href="#license">License</a>
</p> 

![screenshot](https://raw.githubusercontent.com/qjack001/Web-Based-Windows/master/assets/screenshot.png)

## Key Features

For a live preview, visit [qjack001.github.io/Web-Based-Windows/](https://qjack001.github.io/Web-Based-Windows/).

#### Resize windows:

![screenshot](https://raw.githubusercontent.com/qjack001/Web-Based-Windows/master/assets/resize.gif)

#### Move windows:

![screenshot](https://raw.githubusercontent.com/qjack001/Web-Based-Windows/master/assets/move.gif)

#### Close and hide windows:

![screenshot](https://raw.githubusercontent.com/qjack001/Web-Based-Windows/master/assets/close.gif)


## How to Use

To use these windows in your own project, either [fork this repository](https://github.com/qjack001/Web-Based-Windows/fork), or download the required files ([draggable.js](https://github.com/qjack001/Web-Based-Windows/blob/master/draggable.js) and [style.css](https://github.com/qjack001/Web-Based-Windows/blob/master/style.css)) individually.

Add the required files to the `<head>` element of the HTML file, and place any additional scripts or style sheets below:

```html
<head>
  ...
  <link href="https://fonts.googleapis.com/css?family=VT323" rel="stylesheet">
  <link href="style.css" rel="stylesheet" type="text/css">
  <script src="draggable.js" type="text/javascript"></script>
</head>
```

To create a window, set up a new div in the `<body>`. Replace `ADD_CUSTOM_ID` with a new unique ID, and make sure that the div below it has the exact same ID, with `header` added to the end.

```html
<div class="window" id="ADD_CUSTOM_ID"> 
  <div class="window-header" id="ADD_CUSTOM_IDheader"> 
    TITLE_OF_WINDOW 
    <button onclick="this.parentNode.parentNode.style.display = 'none';">X</button> 
    <button onclick="this.parentNode.parentNode.style.display = 'none';">_</button> 
  </div> 
  CONTENTS_OF_WINDOW 
</div> 
<script>dragElement(document.getElementById("ADD_CUSTOM_ID"));</script>
```

Custom window styles can be achieved by importing a separate stylesheet, below the required ones, and appending a newly styled class to the main window's classes. For reference, an [example.html file](https://github.com/qjack001/Web-Based-Windows/blob/master/example.html) has been included in the project.

## Contributing

If you notice a bug or have a feature request, please [submit an issue](https://github.com/qjack001/Web-Based-Windows/issues).
If you would like to contribute to the development of the project, please [create a new pull request](https://github.com/qjack001/Web-Based-Windows/pulls).


## Credits

- [w3schools](https://www.w3schools.com/) - Provided the template for the window's dragging capabilities


## Authors

[**Jack Guinane**](https://github.com/qjack001) - Programming, designing, and maintaining.


## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/qjack001/Web-Based-Windows/blob/master/LICENSE) file for details.

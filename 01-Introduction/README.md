## 01-Getting-Started-Bootstrap

## 1. Introduction to Bootstrap 5

### What is Bootstrap
- Popular CSS Framework
- Completely Free
- Hihgly Customizable
- Responsive Grid System
- Responsive Media Items
- Built-in Components
- Can be Extended

### What's new in Bootstrap 5
- JQuery Removed
- Switched to Vanilla JavaScript
- Custom Font sizes
- Dropped Support or IE 10, IE 11
- Change in Gutter Width
- New Icon Library
- Class Updates

## 2. What you will need
- HTML & CSS
- Windows PC / Linux / MAC
- Android Phone
- Firefox, Chrome, Opera, Edge Browser, Safari

### Code Editor
- Notepad++
- Brackets
- VS Code (Visual Studio Code)
- Sublime Text

## 3. Hello World
- folder: bootstrap

1. create an index.html
2. type html and select the option html:5  
    - this will create the base document structure for our web page
3. import the CDN Bootstrap
    - Now we need to include the  CDN for CSS and JavaScript in the header and the body for our bootstrap document to work
4. https://getbootstrap.com/
5. import the CDN PopperJS
    - next, we need to add another JS file, popperJS helps in loading some bootstrap components like dropdowns, popups and tooltips to load
6. Install Live Server Extension
    - search for the extension and install, then right click the index.html and select open with live server
    - now everytime you update the code the browser will be reloaded

## 4. Bootstrap 5 Document Structure

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bootstrap Web Page</title>  
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css">
</head>
<body>

  <h1>Hello, World!</h1>
   
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

## 5. Quiz 1: Section 1

### Question 1: What is Bootstrap?
- [X] - CSS Framework
- [ ] - JavaScript Framework
- [ ] - Web Design Application
- [ ] - Hosting Platform

### Question 2: What does bootstrap.bundle.min.js include?
- [ ] - JQuery
- [X] - Support for dropdowns, popovers and tooltips
- [ ] - Support for icons
- [ ] - None of above

### Question 3: Bootstrap 5.2 removed the support for?
- [ ] - Google Chrome
- [X] - Internet Explorer 10, & 12
- [ ] - Firefox
- [ ] - Opera

### Question 4: Bootstrap 5.2 supports jQuery?
- [X] - True
- [ ] - False

### Question 5: Bootstrap 5.2 uses vanilla JavaScript?
- [X] - True
- [ ] - False

# Materialize CSS Demo
Materialize is a CSS framework created by Google to provide a good and consistent user experience. Material design was created with cross-platform support in mind, meaning that there are numerous mobile-friendly
features to help ensure that your website looks good and is responsive on any device.

## Getting Started with Materialize CSS:
To get started, you can access the [library](https://materializecss.com/getting-started.html) by including the following two lines in your html file.

* `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css">`
* `<script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/js/materialize.min.js"></script>`

We'll also be including the [jquery](https://cdnjs.com/libraries/jquery) library to utilize some animated JavaScript components for the nav-bar.

* `<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>`

Lastly, we'll include the Google Material icons stylesheet

* `<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`

### Navigation Bar Demo
* To create a nav bar with Material design, we simply have to use the `<nav>` tag and then create a `<div>` inside with the class `nav-wrapper`.
* Materialize provides a pretty decent [Color palette](https://materializecss.com/color.html) for you to stylize with. We can change the color of the nav-bar by defining the class.
* We can then define a logo for our toolbar by using the `<a>` tag and using the class `brand-logo`
* We can now fill in this nav-bar with tabs by creating a list of items.
* We can define where the items are located on the toolbar and its behavior by defining the lists's class, i.e `right hide-on-med-and-down`
* To create the side nav-bar, create a new `div` with the class `sidenav` and give it an id. Then copy and paste the list elements into the side nav.
* We'll then write a short script to tell the web page to switch between the regular toolbar and side toolbar
```
$(document).ready(function(){
 	$('.sidenav').sidenav();
});
```

We now have a good looking and responsive toolbar.
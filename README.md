# ![](http://aptible-media-assets-manual.s3.amazonaws.com/tiny-github-icon.png) aptible-bootstrap-theme

A Bootstrap theme based on our main website, https://www.aptible.com.

### Template  
In the template folder, there is a base template from http://getbootstrap.com/  

a. Like the template, this theme uses:  

- Bootstrap v3.0.3 (css + js)  
- Holder.js v2.2  
- jQuery v1.10.2  

These are the bare minimum files you need. For example, if you're doing a static site, it makes sesnse to just [hit a CDN for them](http://www.bootstrapcdn.com/), although not all CDNs have all the files.

b. If want to use more current versions of these dependencies, be sure to remember that this theme was built on these versions when you debug.

c. The `theme.css` file (which corresponds to `lib/your-custom.css`) is implementing a practice recommended [for fixing the navbar to the top of the page](http://getbootstrap.com/components/#navbar-fixed-top).

d. The stylesheet and script links in the original `getbootstrap.html` were all absolute to http://getbootstrap.com. This template has relative links so you can explore it locally when you pull down this repo. 

### Using This Theme

`aptible-theme.html` contains examples of how you would reference bootstrap elements in your HTML markup. `lib/aptible-theme.css` is the main theme. Make sure you load it *after* Bootstrap, to override the Bootstrap elements.

#### Assets
The `vendor` folder contains the main external files, and the `lib` folder contains the CSS and JS specific to this theme.

#### Performance
You might want to get your `bootstrap.min.css` file from http://getbootstrap.com for performance reasons. I've left the link in comments in the HTML. The getbootstrap domain points to the [twbs GitHub Pages site](https://github.com/twbs/), which looks like it is behind a CDN:

![](img/ghp_performance.png)

You might also swap the jQuery source to [MaxCDN or something](https://oss.maxcdn.com/libs/jquery/1.10.2/jquery.min.js). v1.10.2 doesn't show up in their search results, but it's there. I've included CDN links in the HTML comments.


### To Do:

1. Add more CSS and Javascript examples  
2. Add custom theme  
3. Add custom mixin demos  

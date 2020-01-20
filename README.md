# [HTML parser](https://appseed.us/developer-tools/html-parser)

Interactive tool to convert flat HTML (themes or stand-alone files) to <a href="https://pugjs.org/api/getting-started.html">Pug</a>, <a href="http://jinja.pocoo.org/docs/2.10/">Jinja2</a> and <a href="https://laravel.com/docs/5.8/blade">Blade</a> templates. 

<br />

## What is an HTML Parser

According to Wikipedia, Parsing or syntactic analysis is the process of analyzing a string of symbols, either in natural language or in computer languages, according to the rules of a formal grammar. The meaning of HTML parsing applied here consist into load the HTML, extract and process the relevant information like head title, page assets, main sections and later on, save the processed file.

<br />

## Tool Features
 
The goal of this tool is to automate the UI integration into existing apps, written in different technologies and frameworks. Starting from flat HTML, the tool can be used by anyone to extract components, edit attributes and traverse the HTML tree using an interactive console. 

<br />

## Use-cases 

 - normalize the HTML file to load the assets from a standard directories ( /assets/ [ img, js, css ] ) making the integration in webpack related tools much easier
 - edit / traverse the HTML tree  
 - edit attributes like anchor href's, span texts, remove elements, edit class names 
 - extract components for production use for various engines like PUG, Jinja2, Blade
 - migrate legacy Bootstrap layouts to Bulma and Tailwind CSS frameworks 

<br />

## HTML Parser Work-flow

### Load the HTML theme / page
 
![HTML Parser - Load the HTML theme.](https://github.com/app-generator/static/blob/master/developer-tools/html-parser-select-theme.jpg?raw=true)

![HTML Parser - Select the HTML page.](https://github.com/app-generator/static/blob/master/developer-tools/html-parser-select-file.jpg?raw=true)

<br />

### Select Components

![HTML Parser - Select components.](https://github.com/app-generator/static/blob/master/developer-tools/html-parser-select-component.jpg?raw=true)

<br />

### Edit Elements

![HTML Parser - Edit elements.](https://github.com/app-generator/static/blob/master/developer-tools/html-parser-component-table-view.jpg)

![HTML Parser - Edit elements.](https://github.com/app-generator/static/blob/master/developer-tools/html-parser-component-print-view.jpg?raw=true)

<br />

## Real life sample 

The sample, extracted from [Stellar HTML5Up theme](https://github.com/app-generator/html-parser/tree/master/sample-stellar) is a simple navigation bar, extracted from [this file](https://github.com/app-generator/html-parser/blob/master/sample-stellar/index.html)

- Index file: [original version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/index.html) and [normalized version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/index2.html)
- [JSON descriptor](https://github.com/app-generator/html-parser/blob/master/sample-stellar/index2.json) is generated by the **HTML parser** tool and encapsulate the assets and resources used by the HTML files
- Navigation component
  - [HTML version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/components/nav.html)
  - [PUG version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/components/nav.pug)
  - [Jinja2 Version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/components/nav.j2)
  - [Php version](https://github.com/app-generator/html-parser/blob/master/sample-stellar/components/nav.php)
  - [JSON descriptor](https://github.com/app-generator/html-parser/blob/master/sample-stellar/components/nav.json)
  

### Pug version

```yaml
nav#nav
  ul
    li
      a.active.newclass(href='https://appseed.us/html-parser').
        
        Introduction
        
    li
      a(href='#first').
        
        First Section
        
    li
      a(href='#second').
        
        Second Section
        
    li
      a(href='#cta').
        
        Get Started
```

<br />

### PHP version

```php
<nav id="nav">
 <ul>
  <li>
   <a class="active newclass" href="https://appseed.us/html-parser">
    <?php echo $var_1?>
   </a>
  </li>
  <li>
   <a href="#first">
    <?php echo $var_2?>
   </a>
  </li>
  <li>
   <a href="#second">
    <?php echo $var_3?>
   </a>
  </li>
  <li>
   <a href="#cta">
    <?php echo $var_4?>
   </a>
  </li>
 </ul>
</nav>
```

<br />

## Projects built with this tool 

All are open-source, with live DEMO. 
  - [JAMstack Fractal](https://github.com/app-generator/jamstack-fractal) - HTML5Up design coded in JAMstack pattern
  - [JAMstack BigPicture](https://github.com/app-generator/jamstack-big-picture) - HTML5Up design coded in JAMstack pattern
  - [JAMstack Landed](https://github.com/app-generator/jamstack-landed) - HTML5Up Landed design coded in JAMstack pattern
  - [Flask Dashboard Material Design](https://github.com/app-generator/flask-material-dashboard) - Admin Dashboard with Material Design
  - [Flask Dashboard NowUI](https://github.com/app-generator/flask-now-ui-dashboard) - Admin Dashboard with NowUI Design
  - [Flask Dashboard Black](https://github.com/app-generator/flask-black-dashboard) - Open-Source Admin Panel
  - [Flask Dashboard Argon](https://github.com/app-generator/flask-argon-dashboard) - Open-Source Admin Panel
  - [Flask Dashboard Light](https://github.com/app-generator/flask-dashboard-light-bootstrap) - Open-Source Admin Panel

<br />

## License & Usage
 
**The tool is not open-source**. For licenses, please contact [AppSeed](https://appseed.us/?ref=html-parser) - **support [ @ ] appseed.us**

<br />

---
[HTML parser](https://appseed.us/developer-tools/html-parser) **tool** provided by **AppSeed**

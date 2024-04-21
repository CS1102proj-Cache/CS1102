---
layout: default
---
<head>
     <style>
        .centered-table {
            margin-left: auto;
            margin-right: auto;
        }
        .table-container {
            display: flex;
            justify-content: center;
        }
        .scrollable {
             overflow: auto;
             height: 700px;
        }
    </style>
    <script>
     function greeting() {
         var firstname = prompt("What is your first name?");
         if (firstname !== null && firstname !== "") {
             firstname = firstname[0].toUpperCase() + firstname.substring(1);
             document.getElementById('message').textContent = 'Hello ' + firstname + '! Welcome to our project!';
         } else {
             greeting();
         }
         sessionStorage.setItem("firstname", firstname);
         document.getElementById('firstnamePlaceholder').textContent = firstname;
     }
     function checkvisit() {
          var firstname = sessionStorage.getItem("firstname");
          if (firstname !== null && firstname !== "") {
               document.getElementById('message').textContent = "Welcome back, " + firstname + "!";
               document.getElementById('firstnamePlaceholder').textContent = firstname;
          } else {
               greeting();
          }  
     }     
  </script>
</head>
    
<body onload='checkvisit()'>
 <div id="message"></div>

<div class="bodytext"><div class="middle">
Welcome to our website, <span id="firstnamePlaceholder"></span>! We are going to explore the interesting world of cache memory and its role in accelerating memory input-output (I/O). We will break down concepts like memory types, locality, cache hierarchy, and cache replacement policy. <br/> Join us as we uncover the benefits that cache brings to your computer system. 
<br/><br/>This project is presented by: <br/>
  <div class="centered-table">
    <table class="table-container">
    <thead>
      <tr>
        <th><b>Name</b></th>
        <th><b>SID</b></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Ng Wing Hei</td>
        <td>56612889</td>
      </tr>
      <tr>
        <td>Cheng Man Ho</td>
        <td>56612619</td>
      </tr>
      <tr>
        <td>Lo Wing Sze</td>
        <td>55678893</td>
      </tr>
      <tr>
        <td>Velez Hans Josef Tuble</td>
        <td>56203178</td>
      </tr>
    </tbody>
 </table>
</div>

<br/><br/>

Our project topic is <b>"How Cache Accelerates the Input-Output (I/O) of the Memory"</b>

<br/><br/>

<a href="https://cs1102proj-cache.github.io/CS1102/table_of_contents.html">Click here for <u>Table of Contents.</u></a>
<br/><br/>
<div id="video">
    <iframe width=auto height="315" src="https://www.youtube.com/embed/your-video-id" frameborder="0" allowfullscreen></iframe>
</div>
</div>

<br/><br/>

<div id="method-used">
<h5>Method Used</h5>
     <div class="scrollable">
          <ul>HTML5 doctype declaration: &lt;!DOCTYPE html&gt;</ul>
          <ul>HTML document structure using <code>&lt;</code>html<code>&gt;</code>, <code>&lt;</code>head<code>&gt;</code>, and <code>&lt;</code>body<code>&gt;</code> elements.</ul>
          <ul>Metadata definition using <code>&lt;</code>meta<code>&gt;</code> elements for character encoding and viewport settings.</ul>
          <ul>Linking external resources using <code>&lt;</code>link<code>&gt;</code> elements for fonts and stylesheets.</ul>
          <ul>Customizing styles using <code>&lt;</code>style<code>&gt;</code> blocks and inline CSS.</ul>
          <ul>Creating headings using <code>&lt;</code>h1<code>&gt;</code> to <code>&lt;</code>h6<code>&gt;</code> elements.</ul>
          <ul>Inserting links using <code>&lt;</code>a<code>&gt;</code> elements with the href attribute.</ul>
          <ul>Including placeholders for dynamic content using {{ variable }} syntax.</ul>
          <ul>Defining classes for styling using class attributes.</ul>
          <ul>Wrapping content in <code>&lt;</code>div<code>&gt;</code> elements for organization and styling.</ul>
          <ul>Providing alternative text for accessibility using alt attributes.</ul>
          <ul>Including JavaScript functions using <code>&lt;</code>script<code>&gt;</code> elements.</ul>
          <ul>Including external JavaScript files using <code>&lt;</code>script<code>&gt;</code> elements with the src attribute.</ul>
          <ul>Adding semantic elements like <code>&lt;</code>header<code>&gt;</code>, <code>&lt;</code>main<code>&gt;</code>, and <code>&lt;</code>footer<code>&gt;</code> for better structure and accessibility.</ul>
          <ul>Including skip navigation links using anchor tags with id attributes.</ul>
          <ul>Including comments to document and annotate the code.</ul>
          <ul>Using templating language syntax ({{ variable }}) to insert dynamic content.</ul>
          <ul>Creating dropdown menus using <code>&lt;</code>div<code>&gt;</code> elements with specific classes.</ul>
          <ul>Including images using <code>&lt;</code>img<code>&gt;</code> elements with the src, alt, height, and width attributes.</ul>
          <ul>Creating unordered and ordered lists using <code>&lt;</code>ul<code>&gt;</code> and <code>&lt;</code>ol<code>&gt;</code> elements.</ul>
          <ul>Creating list items using <code>&lt;</code>li<code>&gt;</code> elements.</ul>
          <ul>Nesting lists by placing <code>&lt;</code>ul<code>&gt;</code> or <code>&lt;</code>ol<code>&gt;</code> elements within each other.</ul>
          <ul>Including videos using <code>&lt;</code>iframe<code>&gt;</code> elements with the src attribute.</ul>
          <ul>Using semantic elements like <code>&lt;</code>pre<code>&gt;</code>, <code>&lt;</code>code<code>&gt;</code>, and <code>&lt;</code>hr<code>&gt;</code> for specific content.</ul>
          <ul>Storing and retrieving data in session storage using sessionStorage.setItem() and sessionStorage.getItem().</ul>
          <ul>Capitalizing the first letter of a string using JavaScript string manipulation.</ul>
          <ul>Accessing and modifying HTML elements using the getElementById() method.</ul>
          <ul>Modifying the text content of HTML elements using the textContent property.</ul>
          <ul>Adding a scrolling bar to a section using CSS overflow property.</ul>

</div>

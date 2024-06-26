---
layout: default
---
<head>
     <style>
        .scrollable {
             overflow: auto;
             height: 350px;
             border: 1px dashed #157878 ;
             text-align: left !important;
             border-radius: 5px;
        }
    </style>
    <script src="https://www.youtube.com/iframe_api"></script>
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

<div class="bodytext">
  <div style="text-align: justify; font-size: 20px !important">
Welcome to our website, <span id="firstnamePlaceholder"></span>! We are going to explore the interesting world of cache memory and its role in accelerating memory input-output (I/O). We will break down concepts like memory types, locality, cache hierarchy, and cache replacement policy. <br/> Join us as we uncover the benefits that cache brings to your computer system.
    <br /><br />
  </div>
     This project is presented by: <br/>
    <table>
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

<br/><br/>

Our project topic is <b>"How Cache Accelerates the Input-Output (I/O) of the Memory"</b>

<br/><br/>
You can watch the video for more information and demonstrations.
<br/>
<div id="video"></div>
</div>
<br/><br/>
<a href="https://cs1102proj-cache.github.io/CS1102/table_of_contents.html">Click here for <u>Table of Contents.</u></a>
<br/><br/>
<div id="method-used">
<h5>Method Used (Scroll for more)</h5>
     <div class="scrollable"> <div style="font-size: 16px !important">
          <ul>Adding a scrolling bar to a section using CSS overflow property.</ul>
          <ul>Creating dropdown menus using &lt;div&gt; elements with specific classes.</ul>
          <ul>Embedding YouTube videos using the YouTube IFrame API to autoplay videos.</ul>
          <ul>Using templating language syntax to insert dynamic content.</ul>
          <ul>Storing and retrieving data in session storage using sessionStorage.setItem() and sessionStorage.getItem().</ul>
          <ul>Accessing and modifying HTML elements using the getElementById() method.</ul>
          <ul>Modifying the text content of HTML elements using the textContent property.</ul>
          <ul>HTML5 doctype declaration: &lt;!DOCTYPE html&gt;.</ul>
          <ul>HTML document structure using &lt;html&gt;, &lt;head&gt;, and &lt;body&gt; elements.</ul>
          <ul>Metadata definition using &lt;meta&gt; elements for character encoding and viewport settings.</ul>
          <ul>Linking external resources using &lt;link&gt; elements for fonts and stylesheets.</ul>
          <ul>Customizing styles using &lt;style&gt; blocks and inline CSS.</ul>
          <ul>Creating headings using &lt;h1&gt; to &lt;h6&gt; elements.</ul>
          <ul>Inserting links using &lt;a&gt; elements with the href attribute.</ul>
          <ul>Including placeholders for dynamic content using {{ variable }} syntax.</ul>
          <ul>Defining classes for styling using class attributes.</ul>
          <ul>Wrapping content in &lt;div&gt; elements for organization and styling.</ul>
          <ul>Providing alternative text for accessibility using alt attributes.</ul>
          <ul>Including JavaScript functions using &lt;script&gt; elements.</ul>
          <ul>Including external JavaScript files using &lt;script&gt; elements with the src attribute.</ul>
          <ul>Adding semantic elements like &lt;header&gt;, &lt;main&gt;, and &lt;footer&gt; for better structure and accessibility.</ul>
          <ul>Including skip navigation links using anchor tags with id attributes.</ul>
          <ul>Including comments to document and annotate the code.</ul>
          <ul>Including images using &lt;img&gt; elements with the src, alt, height, and width attributes.</ul>
          <ul>Creating unordered and ordered lists using &lt;ul&gt; and &lt;ol&gt; elements.</ul>
          <ul>Creating list items using &lt;li&gt; elements.</ul>
          <ul>Nesting lists by placing &lt;ul&gt; or &lt;ol&gt; elements within each other.</ul>
          <ul>Including videos using &lt;iframe&gt; elements with the src attribute.</ul>
          <ul>Using semantic elements like &lt;pre&gt;, &lt;code&gt;, and &lt;hr&gt; for specific content.</ul>
          <ul>Capitalizing the first letter of a string using JavaScript string manipulation.</ul>
</div> </div>
<br/>
<br/>
<a href="https://github.com/CS1102proj-Cache/CS1102/blob/main/index.md?plain=1">Click to view the source code of this page.</a>
<br/> <br/> </div>

<script>
  function onYouTubeIframeAPIReady() {
    new YT.Player('video', {
      height: '405',
      width: '720',
      videoId: 'AtLttEk27AE',
      playerVars: {
        autoplay: 0, 
        controls: 1, 
        mute: 0, 
      },
    });
  }
</script>

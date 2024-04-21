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
    </style>
    <script>
     var firstname = localStorage.getItem("firstname");
     function greeting() {
            if (firstname !== "") {
                firstname = firstname[0].toUpperCase() + firstname.substring(1);
                document.getElementById('message').textContent = 'Hello ' + firstname + '! Welcome to our project!';
                localStorage.setItem("firstname", firstname);
            } else {
                var firstname = prompt("What is your first name?");;
            }
        }
     function checkvisit() {
          var firstname = localStorage.getItem("firstname");
          if (firstname == "") { greeting();
          } else {
          document.getElementById('message').textContent = "Welcome back, " + firstname + "!";
     }     
     if (firstname !== null) {
         document.getElementById('firstnamePlaceholder').textContent = firstname;
     }
  </script>
</head>
    
<body onload='checkvisit();greeting();'>
 <div id="message"></div>

<div class="bodytext"><div class="middle">
Welcome to our website, <span id="firstnamePlaceholder"></span>! We are going to explore the interesting world of cache memory and its role in accelerating memory input-output (I/O). We will break down concepts like memory types, locality, cache hierarchy, and cache replacement policy. Join us as we uncover the benefits that cache brings to your computer system. 
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
video
<br/><br/>
method used



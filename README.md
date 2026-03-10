# Ex03 To-Do List using JavaScript
## Date:10-03-2026

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM

### HTML:
```html
<!DOCTYPE html>
<html>
<head>
<title>To Do List</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="container">

<h1>To Do List</h1>

<div class="input-section">
<input type="text" id="taskInput" placeholder="Enter a task">
<button onclick="addTask()">Add</button>
</div>

<ul id="taskList"></ul>

</div>

<script src="script.js"></script>

</body>
</html>
```

### CSS:
```css
body{
font-family: Arial;
background:#f2f2f2;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
}

.container{
background:white;
padding:25px;
border-radius:10px;
width:350px;
box-shadow:0 5px 10px rgba(0,0,0,0.2);
}

h1{
text-align:center;
}

.input-section{
display:flex;
gap:10px;
}

input{
flex:1;
padding:10px;
font-size:16px;
}

button{
padding:10px;
background:#28a745;
border:none;
color:white;
cursor:pointer;
}

button:hover{
background:#218838;
}

ul{
list-style:none;
padding:0;
margin-top:20px;
}

li{
display:flex;
justify-content:space-between;
padding:10px;
border-bottom:1px solid #ddd;
}

.delete{
color:red;
cursor:pointer;
}
```

### JavaScript:
```js
function addTask(){

let input = document.getElementById("taskInput");
let task = input.value;

if(task === ""){
alert("Please enter a task");
return;
}

let li = document.createElement("li");

li.innerHTML = task + '<span class="delete" onclick="deleteTask(this)"> X </span>';

document.getElementById("taskList").appendChild(li);

input.value = "";
}

function deleteTask(element){
element.parentElement.remove();
}
```

## OUTPUT

<img width="1920" height="1080" alt="Screenshot (279)" src="https://github.com/user-attachments/assets/acb74b33-fe9c-4439-95a8-50b97fd9426e" />


<img width="1920" height="1080" alt="Screenshot (280)" src="https://github.com/user-attachments/assets/feddcc9c-271a-4222-9b7a-882c1042c48b" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/16762a1d-0456-443a-acbc-35dc89d06382" />

## RESULT
The program for creating To-do list using JavaScript is executed successfully.

# Static Website: Task Board App

This project was built by implementing the CSS Grid layout & structure to
complete a to-do web app front-end design.

In this project, you will create a board of to-do items organized into columns. All of the HTML and most of the CSS have been written for you, but the grid property declarations have yet to be added.

In order to complete this project, you must know how to lay out the structure of a grid’s rows and columns and place items within that grid using CSS.

We recommend that you review our CSS Grid Lesson 1 before beginning.

![image](https://github.com/abemsq/task-board-app/blob/master/image.png)

## HTML
```
<!DOCTYPE html>
<html>
	<head>
		<title>Project Task Board</title>
		<link rel="stylesheet" type="text/css" href="./style.css"/>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	</head>
	<body>
		<div class="navbar">
			<div class="search-bar">
				<img class="search-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/search_icon.svg">
			</div>
			<h1>STUFFED ANIMAL TASK LIST</h1>
		</div>
		<div class="site-body">
			<div class="container">
				<div class="card-column future-projects">
					<div class="taskgroup-heading">
						<h2>FUTURE PROJECTS</h2>
						<div class="ellipsis-icon">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
						</div>
					</div>
					<div class="card future-i">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Pick Color Trends</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card future-ii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Source Fabrics</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card future-iii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Manufacture clothing</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card future-iv">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Confirm structural integrity</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/23/2017</p>
					</div>
					<div class="card future-v">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Manufacture mandibles</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/26/2017</p>
					</div>
				</div>
				<div class="card-column active-projects">
					<div class="taskgroup-heading">
						<h2>ACTIVE PROJECTS</h2>
						<div class="ellipsis-icon">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
						</div>
					</div>
					<div class="card project-i">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Test fear factor</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card project-ii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Develop button samples</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card project-iii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Recall malfunctioning giraffes</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card project-iv">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">task task task task</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card project-v">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Perform user research on new stuffing</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/23/2017</p>
					</div>
				</div>
				<div class="card-column completed-projects">
				  <div class="taskgroup-heading">
				    <h2>COMPLETED PROJECTS</h2>
				    <div class="ellipsis-icon">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				    </div>
				  </div>
				  <div class="card complete-i">
				    <div class="rectangle yellow"></div>
				    <div class="rectangle green"></div>
				    <div class="rectangle blue"></div>
				    <div class="rectangle orange"></div>
				    <p class="task-description">Research Trends</p>
				    <img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
				    <p class="task-date">4/20/2017</p>
				  </div>
				  <div class="add-card-container">
				    <input class ="new-card-task" placeholder="Add a card...">
				    <button class="add-card">Add</button>
				  </div>
				</div>
			</div>
		</div>
	</body>
</html>
<script>
	$(document).ready(function(){
		$(".add-card").on("click", function(){
			var description = $(".new-card-task").val();
			var today = new Date();
			var dateStr = (today.getMonth()+1) + "/" + today.getDate() + "/" + today.getFullYear();
			var newCard = $(`<div class="card"><div class="rectangle yellow"></div><div class="rectangle green"></div><div class="rectangle blue"></div><div class="rectangle orange"></div><p class="task-description">${description}</p><img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg"><p class="task-date">${dateStr}</p></div>`)
			$(".add-card-container").before(newCard);
		})
	})
</script>


<!DOCTYPE html>
<html>
	<head>
		<title>Project Task Board</title>
		<link rel="stylesheet" type="text/css" href="style.css"/>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	</head>
	<body>
		<div class="navbar">
			<div class="search-bar">
				<img class="search-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/search_icon.svg">
			</div>
			<h1>STUFFED ANIMAL TASK LIST</h1>
		</div>
		<div class="site-body">
			<div class="container">
				<div class="card-column future-projects">
					<div class="taskgroup-heading">
						<h2>FUTURE PROJECTS</h2>
						<div class="ellipsis-icon">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
						</div>
					</div>
					<div class="card future-i">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Pick Color Trends</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card future-ii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Source Fabrics</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card future-iii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Manufacture clothing</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card future-iv">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Confirm structural integrity</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/23/2017</p>
					</div>
					<div class="card future-v">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Manufacture mandibles</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/26/2017</p>
					</div>
				</div>
				<div class="card-column active-projects">
					<div class="taskgroup-heading">
						<h2>ACTIVE PROJECTS</h2>
						<div class="ellipsis-icon">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
							<img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
						</div>
					</div>
					<div class="card project-i">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Test fear factor</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card project-ii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Develop button samples</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card project-iii">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Recall malfunctioning giraffes</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/21/2017</p>
					</div>
					<div class="card project-iv">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">task task task task</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/20/2017</p>
					</div>
					<div class="card project-v">
						<div class="rectangle yellow"></div>
						<div class="rectangle green"></div>
						<div class="rectangle blue"></div>
						<div class="rectangle orange"></div>
						<p class="task-description">Perform user research on new stuffing</p>
						<img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
						<p class="task-date">4/23/2017</p>
					</div>
				</div>
				<div class="card-column completed-projects">
				  <div class="taskgroup-heading">
				    <h2>COMPLETED PROJECTS</h2>
				    <div class="ellipsis-icon">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				       <img src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/oval-copy.svg">
				    </div>
				  </div>
				  <div class="card complete-i">
				    <div class="rectangle yellow"></div>
				    <div class="rectangle green"></div>
				    <div class="rectangle blue"></div>
				    <div class="rectangle orange"></div>
				    <p class="task-description">Research Trends</p>
				    <img class="list-icon" src="https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/list_icon.svg">
				    <p class="task-date">4/20/2017</p>
				  </div>
				  <div class="add-card-container">
				    <input class ="new-card-task" placeholder="Add a card...">
				    <button class="add-card">Add</button>
				  </div>
				</div>
			</div>
		</div>
	</body>
</html>
<script>
	$(document).ready(function(){
		$(".delete-card").on("click", function(){
			var description = $(".delete-card-task").val();
			var today = new Date();
			$(".delete-card-container").before(newCard);
		})
	})
</script>
```

## CSS
```
@font-face {
	font-family: WorkSans;
	src: url("https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/Work_Sans/WorkSans-Regular.ttf");
}
@font-face {
	font-family: Poppins;
	src: url("https://s3.amazonaws.com/codecademy-content/courses/learn-css-grid/project-ii/Resources/Poppins/Poppins-Regular.ttf");
}

html {
    height: 100%;
}
body {
    height: 100%;
    margin: 0;
    background-image: linear-gradient(359deg, #3023ae, #eb7f7b);
    background-repeat: no-repeat;
    background-attachment: fixed;
}

.navbar {
    display: grid;
    grid-template-columns: 10px 1fr 3fr 1fr;
    position: absolute;
    width: 100%;
    height: 60px;
    background-color: rgba(120,70,154, 0.2);
    text-align: center;
    top: 0;
    left: 0;
    justify-content: space-around;
}

.navbar h1 {
	font-family: Poppins;
    color: #ffffff;
    margin: 0;
    align-self: center;
}

.container {
	width: 1000px;
	display: grid;
	grid-template-columns: 1fr 1fr 1fr;
	grid-gap: 20px;
}

.search-bar {
	height: 40px;
    background-color: rgba(255,255,255, 0.35);
    align-self: center;
    grid-column-start: 2;
}

input {
	display: inline-block;
	border: none;
	background: transparent;
	font-size: 14px;
}

.search-bar input {
	float: left;
	height: 18px;
    margin-top: 9px;
    margin-left: 7px;	
}

.card-column input {
	height: 18px;
    margin-left: 15px;		
}

.search-icon {
	float: left;	
    margin-top: 9px;
    margin-left: 7px;
}

.card-column {
	background-color: #ffffff;
	display: grid;
	grid-gap: 10px;
	grid-template-rows: 20px repeat(6, 100px);
}

.card-column h2 {
	padding: 0;
    margin: 0 auto;
    font-family: WorkSans;
    font-size: 16px;
	font-weight: 600;
	letter-spacing: 0.2px;
	text-align: left;
	color: #2f2f2f;
	display: inline-block;
}

.taskgroup-heading {
	margin-left: 15px;
	margin-top: 7px;
}

.site-body {
	position: absolute;
	top: 100px;
	margin-left: 50px;
}

.card {
	margin-right: 15px;
	margin-left: 15px;
	background-color: rgba(216, 216, 216, 0.21);
	border: solid 1px rgba(151,151,151,0.21);
	position: relative;
}

.rectangle {
  width: 57px;
  height: 6px;
  position: relative;
  display: inline-block;
  margin-left: 7px;
}

.list-icon {
	display: inline-block;
	margin-left: 7px;
	margin-bottom: 5px;
	position: absolute;
	bottom: 0;
}

.task-description {
	margin-left: 7px;
	margin-top: 0;
	font-family: WorkSans;
	font-size: 14px;
	letter-spacing: 0.2px;
	text-align: left;
	color: #2f2f2f;
}

.ellipsis-icon {
	display: inline-block;
	float: right;
    margin-right: 15px;
}

.task-date {
	display: inline-block;
	font-family: WorkSans;
	font-size: 10px;
	letter-spacing: 0.1px;
	text-align: left;
	color: #9b9b9b;
	position: absolute;
    bottom: 0;
    margin-bottom: 5px;
    left: 25px;
}

.yellow {
	background-color: #fdcb1e;
}

.orange {
	background-color: #ff7700;
}

.green {
	background-color: #50e3c2;
}

.blue {
	background-color: #3343e5;
}

.add-card {
	background-color: rgba(216, 216, 216, 0.21);
    border: solid 1px rgba(151,151,151,0.21);
    color: #2f2f2f;
}

.delete-card {
	background-color: rgba(216, 216, 216, 0.21);
    border: solid 1px rgba(151,151,151,0.21);
    color: #2f2f2f;
}

.completed-projects {
	grid-template-rows: 20px;
	grid-auto-rows: 100px;
}
```
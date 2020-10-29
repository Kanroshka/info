Клонирование проектав папку в папку nameProject:
git clone https://...nameProject

Добавление файлов в коммит:
git add . 

Запись коммита:
git commit -m "Коментарий коммита"

Отправить коммит:
git push 

Принять изменения:
git pull

Авторство коммитов:
git config --global user.email "Ваш емайл"
git config --global user.name "Ваш Имя"

Домашняя работа

<!DOCTYPE html>
<html>
	<head>
		<style>
		</style>
	</head>
	<body>
		<div class=''></div>

		<script type='tex/javascript'></script>
	</body>
</html>


1)


<html>
<head>
	<link rel="stylesheet" type="text/css" href="./public/styles/style.css">	
</head>
<body id="body">
	<div id="time"></div>
	<script type="text/javascript" src="./public/scripts/main.js">
	</script>
</body>
</html>

2)
body {
	background-color: black;
	margin: 0;
	padding: 0;
}

#time {
	text-align: center;
	color: white;
	font-size: 144px;
	font-family: Arial;
	font-weight: 500;
}

3)
setInterval(() => {
	var date = new Date();
	var hour = String(((date.getHours() * 4) < 10 ? '0' + (date.getHours() * 4) : (date.getHours() * 4)));
	var min = String((date.getMinutes() < 10 ? '0' + date.getMinutes() : date.getMinutes()));
	var sec = String((date.getSeconds() < 10 ? '0' + date.getSeconds() : date.getSeconds()));
	var timeColor = '#' + hour + min + sec;
	console.log(timeColor);

	var time = hour + ':' + min + ':' + sec;



	document.getElementById('body').style.backgroundColor = timeColor;
	document.getElementById('time').innerText = time;

}, 1);



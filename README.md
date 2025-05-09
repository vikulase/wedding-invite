# wedding-invite
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"
/>
<title>Свадьба Сергея и Виктории</title>
<style>
body {
margin: 0;
font-family: 'Times New Roman', serif;
background-color:
color: #333;
text-align; center;
header {
background-color: #f8f8f8;
padding: 40px 20px 20px;
header img {
width: 100px;
margin: 10px;
}
h1 {
font-size; 2,5em;
margin: 0;
h2 color: #777;
font-size: 1.2em;
section {
padding: 30px 20px;
max-width; 600px;
margin: 0 auto;
.countdown {
font-size: 1.5em;
margin-top: 20px; color: #6b8e23;
form { display: flex; дар: 15px; margin-top: 20px;
flex-direction; column;
input, select, button { padding: 10px;
font-size: 1em;
border: 1px solid #ссс;
border-radius: 8px;
button {
background-color: #6b8e23;
color: white;
border; none;
cursor: pointer;
}
button: hover
background-color: #557a1f;
}
dress-code {
margin-top: 30px;
padding: 20px;
background-color: #f2f2f2;
border-radius: 10px;
.color-samples {
display: flex;
justify-content: center;
дар: 10px;
margin-top: 10px;
}
.color-box
width: 40px;
height: 40px;
border-radius: 50%;
border; 2px solid #ссс;
</style>
</head>
<body>
<header>
<img src="https://upload, wikimedia.org/wikipedia/commons/thumb/4/4f/
Olive-branch.svg/240px-Olive-branch,svg.png" alt="Оливковая ветвь">
<img src="https://upload, wikimedia.org/wikipedia/commons/thumb/5/5f/
Wedding_rings_icon.svg/240px-Wedding_rings_icon.svg.png" alt="Обручальные кольца">
<h1>Сергей & Виктория</h1>
<h2>25 июля 2025</h2>
<div class="countdown" id="countdown"></div>
</header>
<section>
<h2>Дорогие и уважаемые гости!</h2>
<p>С радостью приглашаем вас на наше торжество!</p>
<p>Сбор гостей возле ЗАГСа</p>
<p>Регистрация брака: 15:00 - Ивнянский ЗАГС</p>
<p>Банкет: 17:00 - кафе "ЛИДЕР"</p>
</section>
<section>
<h2>С уважением просим</h2>
<p>Вместо цветов подарить нам бутылочку вина или шампанского - мы будем благодарны!</p>
<p>Также, по возможности, просим воздержаться от криков "Горько" - пусть наши поцелуи будут искренними и по вдохновению сердца,</р>
</section>
<section class="dress-code">
<h2>Дресс-код</h2>
<p>Будем признательны, если выберете наряды в следующих цветах:</p>
<div class="color-samples">
<div class="color-box" style="background-color: #F5CB8B" title="#F5C383"></div>
<div class="color-box" style="background-color: #E5D64C" title="#E5D64C"></div>
<div class="color-box" style="background-color: #913745D" title="#913745D"></div>
<div class="color-box" style="background-color: #74C8FF" title="#74C8FF"></div>
<div class="color-box" style="background-color: #E690FF" title="#E690FF"></div>
</div>
</section>
<section>
<h2>Подтвердите участие</h2>
<form>
<input type="text" placeholder="Baшe имя" required> <select required>
<option value="">Вы будете присутствовать?</option>
<option value="yes">Да</option>
<option value="no">Нет</option>
</select>
<select required>
<option value="">Будете ли вы с детьми?</option>
<option value="with-children">Да</option>
<option value="no-children">Нет</option>
</select>
<button type="submit">Отправить</button>
</form>
</section>
<script>
// Обратный отсчёт const countdownElement = document.getElementById('countdown'); const weddingDate = new Date('2025-07-25T00:00:00');
function updateCountdown() { const now = new Date(); const diff = weddingDate - now;
if (diff<= 0){
countdownElement.textContent = 'Свадьба уже состоялась!'; return;
}
const days = Math,floor(diff / (1000 * 60 * 60 * 24)); const hours = Math.floor((diff / (1000 * 60 * 60)) % 24); const minutes = Math.floor((diff / (1000 * 60)) % 60);
countdownElement,textContent = До свадьбы осталось: ${days} дн. ${hours}
ч. ${minutes} мин. ;
}
updateCountdown();
setInterval(updateCountdown, 60000);
</script>
</body>
</html>

<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Контакты партнёров</title>

<style>

/* Общие настройки */
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f5f7f8;
    color: #1d352b;
}

.widget {
    padding: 20px;
}

/* Заголовок */
h2 {
    margin: 0 0 20px;
    color: #1d352b;
}

/* Вкладки */
.tabs {
    display: flex;
    gap: 10px;
    margin-bottom: 20px;
}

.tab {
    border: none;
    padding: 12px 18px;
    border-radius: 10px;
    cursor: pointer;
    font-size: 15px;
    background: #e9ecef;
    color: #1d352b;
}

.tab.active {
    background: #0f7d46;
    color: white;
}

/* Поиск */
#search {
    width: 100%;
    padding: 12px;
    border-radius: 10px;
    border: 1px solid #ddd;
    font-size: 15px;
    margin-bottom: 20px;
}

/* Карточка */
.card {
    background: white;
    padding: 18px;
    margin-bottom: 15px;
    border-radius: 14px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, .05);
}

.card h3 {
    margin: 0 0 12px;
    color: #0f7d46;
}

.card p {
    margin: 0 0 4px;
}

.card a {
    display: block;
    margin-top: 6px;
    text-decoration: none;
    color: #0f7d46;
    font-weight: 600;
    word-break: break-word;
}

/* Имя куратора + плашка с днём рождения */
.name {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 10px;
}

.birthday-box {
    flex-shrink: 0;
    display: flex;
    flex-direction: column;
    text-align: center;
}

.birthday-label {
    margin-bottom: 3px;
    font-size: 11px;
    color: #1d352b;
    white-space: nowrap;
}

.birthday {
    padding: 4px 10px;
    border-radius: 20px;
    background: #0f7d46;
    color: white;
    font-size: 13px;
    white-space: nowrap;
}

/* Разделитель между сотрудниками в одной карточке */
.person + .person {
    margin-top: 16px;
    padding-top: 16px;
    border-top: 1px solid #eee;
}

/* Город */
.note {
    margin-top: 12px;
    padding: 10px;
    background: #f2f2f2;
    border-radius: 8px;
    font-size: 13px;
}

/* Содержимое вкладок */
.tab-content {
    display: none;
}

.tab-content.active {
    display: block;
}

/* Во время поиска показываем обе вкладки */
.searching .tab-content {
    display: block;
}

</style>
</head>

<body>

<div class="widget" id="widget">

<h2>Контакты партнёров</h2>

<!-- Вкладки -->
<div class="tabs">
    <button type="button" class="tab active" onclick="openTab('banks', this)">
        Банки
    </button>

    <button type="button" class="tab" onclick="openTab('insurance', this)">
        Страхование
    </button>
</div>

<!-- Поиск -->
<input
    id="search"
    type="text"
    placeholder="Поиск банка, компании или менеджера"
/>


<!-- БАНКИ -->
<div id="banks" class="tab-content active">

<!-- Абсолютбанк -->
<div class="card">
    <h3>Абсолютбанк</h3>

    <div class="person">
        <p class="name"><b>Кенжибаева Надима Батыровна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">20 сентября</span></span></p>
        <p>Начальник управления партнерских программ</p>
        <a href="tel:+79117755786">+7 911 775-57-86</a>
        <a href="mailto:ipoteka_spb@absolutbank.ru">ipoteka_spb@absolutbank.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- АкБарсБанк -->
<div class="card">
    <h3>АкБарсБанк</h3>

    <div class="person">
        <p><b>Каюмова Ольга Юрьевна</b></p>
        <p>Менеджер направления партнерского канала Западного РЦ</p>
        <a href="tel:+79219881237">+7 921 988-12-37</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Альфа-банк, Москва -->
<div class="card">
    <h3>Альфа-банк</h3>

    <div class="person">
        <p><b>Маркушов Павел</b></p>
        <a href="tel:+79167868181">+7 916 786-81-81</a>
        <a href="mailto:pmarkushov@alfabank.ru">pmarkushov@alfabank.ru</a>
    </div>

    <div class="note">Москва</div>
</div>

<!-- Альфа-банк, Санкт-Петербург -->
<div class="card">
    <h3>Альфа-банк</h3>

    <div class="person">
        <p class="name"><b>Мельник Карина</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">3 июня</span></span></p>
        <a href="tel:+79616357744">+7 961 635-77-44</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- БЖФ -->
<div class="card">
    <h3>БЖФ</h3>

    <div class="person">
        <p><b>Ольга Александрович</b></p>
        <p>Руководитель регионального развития партнерских продаж</p>
        <a href="tel:+79127993911">+7 912 799-39-11</a>
        <a href="mailto:o.aleksandrovich@bgf-bank.ru">o.aleksandrovich@bgf-bank.ru</a>
    </div>

    <div class="person">
        <p><b>Гирева Оксана Владимировна</b></p>
        <a href="tel:+79250078053">+7 925 007-80-53</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- ВТБ -->
<div class="card">
    <h3>ВТБ</h3>

    <div class="person">
        <p class="name"><b>Коханчук Роман Олегович</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">11 июня 1989</span></span></p>
        <p>Эксперт отдела развития ипотечного бизнеса</p>
        <a href="tel:+79110252566">+7 911 025-25-66</a>
        <a href="mailto:kokhanchukroman@yandex.ru">kokhanchukroman@yandex.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Дом.рф -->
<div class="card">
    <h3>Дом.рф</h3>

    <div class="person">
        <p class="name"><b>Окорокова Вера Владимировна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">6 февраля 1989</span></span></p>
        <p>Руководитель направления | Развитие партнерских продаж</p>
        <a href="tel:+79213963818">+7 921 396-38-18</a>
        <a href="mailto:vera.okorokova@domrf.ru">vera.okorokova@domrf.ru</a>
    </div>

    <div class="person">
        <p><b>Берштейн Роман</b></p>
        <a href="mailto:roman.bershtein@domrf.ru">roman.bershtein@domrf.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Металлинвестбанк -->
<div class="card">
    <h3>Металлинвестбанк</h3>

    <div class="person">
        <p class="name"><b>Максимова Екатерина Рахатовна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">15 августа</span></span></p>
        <p>Главный специалист по работе с партнерами Центр ипотечного кредитования|Департамент ипотечного кредитования</p>
        <a href="tel:+79265787297">+7 926 578-72-97</a>
        <a href="mailto:emaksimova@metib.ru">emaksimova@metib.ru</a>
    </div>

    <div class="note">Москва</div>
</div>

<!-- МКБ, Москва -->
<div class="card">
    <h3>МКБ</h3>

    <div class="person">
        <p class="name"><b>Лукьянова Татьяна Владимировна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">18 марта</span></span></p>
        <p>Руководитель направления по работе с Партнерами</p>
        <a href="tel:+79035264600">+7 903 526-46-00</a>
        <a href="mailto:LukyanovaTV@mkb.ru">LukyanovaTV@mkb.ru</a>
    </div>

    <div class="note">Москва</div>
</div>

<!-- МКБ, Санкт-Петербург -->
<div class="card">
    <h3>МКБ</h3>

    <div class="person">
        <p class="name"><b>Маркин Виталий Владимирович</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">25 января</span></span></p>
        <p>Территориальный директор</p>
        <a href="tel:+79111820237">+7 911 182-02-37</a>
        <a href="mailto:MarkinV@mkb.ru">MarkinV@mkb.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- ПримСоцБанк -->
<div class="card">
    <h3>ПримСоцБанк</h3>

    <div class="person">
        <p class="name"><b>Пальшина Евгения Васильевна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">13 декабря</span></span></p>
        <p>Главный менеджер активных продаж Сектора продаж</p>
        <a href="tel:+79816978781">+7 981 697-87-81</a>
        <a href="mailto:palshina_ev@pskb.com">palshina_ev@pskb.com</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Промсвязьбанк -->
<div class="card">
    <h3>Промсвязьбанк</h3>

    <div class="person">
        <p class="name"><b>Шебалов Владимир</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">30 апреля</span></span></p>
        <a href="tel:+79214261567">+7 921 426-15-67</a>
        <a href="mailto:shebalovvv@spb.psbank.ru">shebalovvv@spb.psbank.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Реалист Ипотека (ранее Ипотека 24) -->
<div class="card">
    <h3>Реалист Ипотека (ранее Ипотека 24)</h3>

    <div class="person">
        <p><b>Ячменева Наталья</b></p>
        <p>Руководитель ипотечного центра</p>
        <a href="tel:+79819622779">+7 981 962-27-79</a>
    </div>

    <div class="person">
        <p class="name"><b>Васильева Ирина</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">17 июня 1969</span></span></p>
        <a href="tel:+79213200913">+7 921 320-09-13</a>
        <a href="mailto:i.vasileva@realistipoteka.ru">i.vasileva@realistipoteka.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Россельхозбанк -->
<div class="card">
    <h3>Россельхозбанк</h3>

    <div class="person">
        <p class="name"><b>Соколова Виктория Александровна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">30 октября</span></span></p>
        <p>Главный менеджер отдела развития партнерских продаж Санкт-Петербургского регионального филиала АО Россельхозбанк</p>
        <a href="tel:+79112192118">+7 911 219-21-18</a>
        <a href="mailto:SokolovaVA@spb.rshb.ru">SokolovaVA@spb.rshb.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Россия -->
<div class="card">
    <h3>Россия</h3>

    <div class="person">
        <p class="name"><b>Бровков Василий Павлович</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">13 февраля 1989</span></span></p>
        <p>Руководитель направления по ипотечному кредитованию</p>
        <a href="tel:+79878384527">+7 987 838-45-27</a>
        <a href="mailto:v.p.brovkov@abr.ru">v.p.brovkov@abr.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Санкт-Петербург -->
<div class="card">
    <h3>Санкт-Петербург</h3>

    <div class="person">
        <p class="name"><b>Екатерина Сухоребрикова</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">19 апреля</span></span></p>
        <p>Руководитель направления группы ипотечного кредитования и расчетов по сделкам с недвижимостью</p>
        <a href="tel:+79219641758">+7 921 964-17-58</a>
        <a href="mailto:Ekaterina.v.suhorebrikova@bspb.ru">Ekaterina.v.suhorebrikova@bspb.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Совкомбанк, Санкт-Петербург -->
<div class="card">
    <h3>Совкомбанк</h3>

    <div class="person">
        <p class="name"><b>Калашник Юлия Владимировна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">2 марта 1990</span></span></p>
        <p>Менеджер по продажам по ипотечному кредитованию, Управление по г. Санкт-Петербургу и Калининградской области</p>
        <a href="tel:+79813003604">+7 981 300-36-04</a>
        <a href="mailto:kalashnikyv@sovcombank.ru">kalashnikyv@sovcombank.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Совкомбанк, Москва -->
<div class="card">
    <h3>Совкомбанк</h3>

    <div class="person">
        <p class="name"><b>Лукин Алексей Андреевич</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">27 января</span></span></p>
        <p>Руководитель направления по развитию бизнеса, Отдел сопровождения финансовых продуктов</p>
        <a href="tel:+79629752509">+7 962 975-25-09</a>
        <a href="mailto:lukinaa@sovcombank.ru">lukinaa@sovcombank.ru</a>
    </div>

    <div class="note">Москва</div>
</div>

<!-- Сургутнефтегазбанк -->
<div class="card">
    <h3>Сургутнефтегазбанк</h3>

    <div class="person">
        <p class="name"><b>Денисова Ольга Николаевна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">24 декабря</span></span></p>
        <p>Руководитель направления по ипотечному кредитованию</p>
        <a href="tel:+79217571861">+7 921 757-18-61</a>
    </div>

    <div class="person">
        <p><b>Документы высылать на почту</b></p>
        <a href="mailto:sngb-spf@sngb.ru">sngb-spf@sngb.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

<!-- Транскапиталбанк -->
<div class="card">
    <h3>Транскапиталбанк (ТКБ)</h3>

    <div class="person">
        <p class="name"><b>Ермолаев Дмитрий</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">19 марта</span></span></p>
        <a href="tel:+79277297846">+7 927 729-78-46</a>
        <a href="mailto:ermolaev_dv@tkbbank.ru">ermolaev_dv@tkbbank.ru</a>
    </div>

    <div class="note">Самара</div>
</div>

<!-- Уралсиб -->
<div class="card">
    <h3>Уралсиб</h3>

    <div class="person">
        <p class="name"><b>Краснова Ольга Михайловна</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">27 июля</span></span></p>
        <p>Начальник отдела ипотечного кредитования, Филиал ПАО "БАНК УРАЛСИБ" в г. Санкт-Петербург</p>
        <a href="tel:+79046051530">+7 904 605-15-30</a>
    </div>

    <div class="person">
        <p class="name"><b>Ирина</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">27 июля</span></span></p>
        <a href="tel:+79247829995">+7 924 782-99-95</a>
    </div>

    <div class="person">
        <p><b>Документы высылать на почту</b></p>
        <a href="mailto:zik@spb.uralsib.ru">zik@spb.uralsib.ru</a>
    </div>

    <div class="note">Санкт-Петербург</div>
</div>

</div>
<!-- /БАНКИ -->


<!-- СТРАХОВАНИЕ -->
<div id="insurance" class="tab-content">

<!-- АльфаСтрахование -->
<div class="card">
    <h3>АльфаСтрахование</h3>

    <div class="person">
        <p class="name"><b>Лозовая Мария</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">1 февраля</span></span></p>
        <a href="mailto:lozovaiamv@alfastrah.ru">lozovaiamv@alfastrah.ru</a>
    </div>

    <div class="person">
        <p class="name"><b>Марина</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">10 сентября</span></span></p>
    </div>
</div>

<!-- ВСК -->
<div class="card">
    <h3>ВСК</h3>

    <div class="person">
        <p><b>Голубева Ульяна</b></p>
        <a href="mailto:ugolubeva@vsk.ru">ugolubeva@vsk.ru</a>
    </div>

    <div class="person">
        <p><b>Жукова Мария</b></p>
    </div>

    <div class="person">
        <p><b>Гриценко Елена</b></p>
    </div>
</div>

<!-- Ингосстрах -->
<div class="card">
    <h3>Ингосстрах</h3>

    <div class="person">
        <p><b>Кузнецова Ольга</b></p>
        <a href="tel:+79213696348">+7 921 369-63-48</a>
        <a href="mailto:Olga.V.Kuznetsova@ingos.ru">Olga.V.Kuznetsova@ingos.ru</a>
    </div>
</div>

<!-- Ренессанс -->
<div class="card">
    <h3>Ренессанс</h3>

    <div class="person">
        <p class="name"><b>Сиренко Оксана</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">29 сентября</span></span></p>
    </div>
</div>

<!-- Росгосстрах -->
<div class="card">
    <h3>Росгосстрах</h3>

    <div class="person">
        <p class="name"><b>Кузнецова Екатерина</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">16 февраля</span></span></p>
    </div>

    <div class="person">
        <p class="name"><b>Логинова Ольга</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">5 мая</span></span></p>
    </div>

    <div class="person">
        <p><b>Бойко Алексей</b></p>
    </div>

    <div class="person">
        <p><b>Дарья</b></p>
    </div>
</div>

<!-- Согласие -->
<div class="card">
    <h3>Согласие</h3>

    <div class="person">
        <p><b>Анна</b></p>
        <a href="tel:+79500050421">+7 950 005-04-21</a>
        <a href="mailto:anna.berezkina@soglasie.ru">anna.berezkina@soglasie.ru</a>
    </div>

    <div class="person">
        <p><b>Даниил</b></p>
    </div>

    <div class="person">
        <p><b>Елизавета</b></p>
    </div>

    <div class="person">
        <p><b>Исаковская Ольга</b></p>
    </div>

    <div class="person">
        <p><b>Ната</b></p>
    </div>

    <div class="person">
        <p><b>Ксения</b></p>
    </div>
</div>

<!-- Югория -->
<div class="card">
    <h3>Югория</h3>

    <div class="person">
        <p class="name"><b>Шустер Ольга</b><span class="birthday-box"><span class="birthday-label">День рождения</span><span class="birthday">15 июля</span></span></p>
    </div>
</div>

</div>
<!-- /СТРАХОВАНИЕ -->

</div>


<script>

const widget = document.getElementById('widget');
const search = document.getElementById('search');
const cards = document.querySelectorAll('.card');

/* Переключение вкладок (поиск при этом сбрасывается) */
function openTab(tab, button) {
    document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
    document.querySelectorAll('.tab').forEach(el => el.classList.remove('active'));

    document.getElementById(tab).classList.add('active');
    button.classList.add('active');

    search.value = '';
    filterCards();
}

/* Приводим текст к одному виду: нижний регистр, ё = е */
function normalize(text) {
    return text.toLowerCase().replace(/ё/g, 'е');
}

/* Поиск по всему тексту карточки: банк, ФИО, должность, телефон, почта, город */
function filterCards() {
    const value = normalize(search.value.trim());

    widget.classList.toggle('searching', value !== '');

    cards.forEach(card => {
        card.style.display = normalize(card.textContent).includes(value) ? '' : 'none';
    });
}

search.addEventListener('input', filterCards);

</script>

</body>
</html>

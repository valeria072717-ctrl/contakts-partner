<h2>Контакты партнёров</h2>

<div class="tabs">
    <button class="tab active" onclick="openTab('banks')">
        Банки
    </button>

    <button class="tab" onclick="openTab('insurance')">
        Страхование
    </button>
</div>

<input
id="search"
type="text"
placeholder="Поиск банка, компании или менеджера"
/>


<!-- БАНКИ -->

<div id="banks" class="tab-content active">

<div class="card" data-search="абсолютбанк ипотека Надима">
    <h3>Абсолютбанк</h3>

    <p><b>Надима Батыровна</b></p>
    <p>Начальник управления партнерских программ</p>

    <a href="tel:+7900000000">
        +7 911 775-57-86
    </a>

    <a href="mailto:test@test.ru">
        n.kenzhebaeva@absolutbank.ru
    </a>

    <div class="note">
        Санкт-Петербург
    </div>
</div>

<div class="card" data-search="абсолютбанк ипотека Надима">
    <h3>АкБарсБанк</h3>

    <p><b>Каюмова Ольга Юрьевна</b></p>
    <p>Менеджер направления партнерского канала Западного РЦ</p>

    <a href="tel:+7900000000">
        +7 921 988-12-37
        +7 981 112-41-26
    </a>

    <a href="mailto:test@test.ru">
        olga.kayumova@akbars.ru
    </a>

    <div class="note">
        Санкт-Петербург
    </div>
</div>

<div class="card" data-search="альфа-банк Александр">
    <h3>Альфа-банк</h3>

    <p><b>Лукин Александр Андреевич</b></p>
    <p>Главный менеджер по работе с партнерами/Дирекция развития ипотечных продаж/Управление по продажам в МиМо</p>

    <a href="tel:+7900000000">
        +7 909 663-27-48
    </a>

    <a href="mailto:test@test.ru">
        aalukin@alfabank.ru
    </a>
    <div class="note">
        Москва
    </div>
</div>

<div class="card" data-search="альфа-банк Татьяна">
    <h3>Альфа-банк</h3>

    <p><b>Бардамаева Татьяна</b></p>
    <p>Главный менеджер по работе с партнерами Альфа-Банка</p>

    <a href="tel:+7900000000">
        +7 904 336-06-84
    </a>

    <a href="mailto:test@test.ru">
        TBardamaeva@alfabank.ru
    </a>
    <div class="note">
        Санкт-Петербург
    </div>
</div>

<!-- СТРАХОВАНИЕ -->

<div id="insurance" class="tab-content">

<div class="card"
data-search="альфастрахование">

<h3>АльфаСтрахование</h3>

<p><b>Ольга Иванова</b></p>

<p>Страховой менеджер</p>

<a href="tel:+7900000000">
+7 900 000-00-00
</a>

<a href="mailto:test@test.ru">
test@test.ru
</a>

</div>



<div class="card"
data-search="ингосстрах">

<h3>Ингосстрах</h3>

<p><b>Анна Соколова</b></p>

<p>Партнёрский отдел</p>

<a href="tel:+7900000000">
+7 900 000-00-00
</a>

<a href="mailto:test@test.ru">
test@test.ru
</a>

</div>

</div>

</div>



<style>

body{

margin:0;
font-family:Arial;
background:#f5f7f8;

}


.widget{

padding:20px;

}


.header h2{

margin-bottom:20px;
color:#1d352b;

}



.tabs{

display:flex;
gap:10px;
margin-bottom:20px;

}


.tab{

border:none;
padding:12px 18px;
border-radius:10px;
cursor:pointer;

background:#e9ecef;

}


.tab.active{

background:#0f7d46;
color:white;

}



#search{

width:100%;
padding:12px;
border-radius:10px;
border:1px solid #ddd;

margin-bottom:20px;

}



.card{

background:white;
padding:18px;

margin-bottom:15px;

border-radius:14px;

box-shadow:
0 4px 15px rgba(0,0,0,.05);

}


.card h3{

margin-top:0;
color:#0f7d46;

}


.card a{

display:block;
margin-top:10px;

text-decoration:none;

color:#0f7d46;

font-weight:600;

}


.note{

margin-top:10px;

padding:10px;

background:#f2f2f2;

border-radius:8px;

font-size:13px;

}



.tab-content{

display:none;

}


.tab-content.active{

display:block;

}

</style>



<script>

function openTab(tab){

document
.querySelectorAll('.tab-content')
.forEach(el =>
el.classList.remove('active')
);

document
.querySelectorAll('.tab')
.forEach(el =>
el.classList.remove('active')
);


document
.getElementById(tab)
.classList.add('active');


event.target
.classList.add('active');

}



document
.getElementById('search')
.addEventListener('input',function(){

let value =
this.value.toLowerCase();

document
.querySelectorAll('.card')
.forEach(card=>{

let text =
card.dataset.search;

card.style.display =
text.includes(value)
?
'block'
:
'none';

})

})

</script>

# Grease Monkey Manager

Приветствую.

Ознакомится с проектом и поклацать можно <a href='http://grmonkey.site'>тут</a>
 Тестовый аккаунт: mihaker01@gmail.com , 111111

<h4>Что это?</h4>
<p>
  Это небольшое SPA приложение для личного учёта заработка автослесаря работающего на станции техобслуживания автомобилей,
  оклад которого расчитывается процентом от выработки. Эдакая CRM-ка для механика.
  
  Построено на MERN стеке с использованием Redux, и функциональных компонентов. В качестве БД используется бесплатный Atlas MongoDB.
  Верстка в приложении ориентирована только на мобильные телефоны. Использование десктопа по моему мнению бессмысленно.
  Не смотря на это на нем верстка не разваливается и пользоваться можно и с декстопа.
</p>


<h4>Зачем все это?</h4>

<i>Небольшое отступление. Я сам пока что работаю автослесарем и писал приложение для себя, но старался подстроить его и под "коллег по цеху".</i>
<p>
  Приложение позволяет записывать (или указывать из предустановленных вариантов) выполненные работы по автомобилю:
  что сделано, когда сделано и стоимость работ до вычета процента. Так же имеется статистика по неделям и месяцам.
</p>
<h4>Что реализовано</h4>
<ul>
  <li>Реализована регистрация (эмейл в качестве логина) и авторизация через jwt токен.</li>
  <li>Реализована (довольно примитивная) функция восстановления доступа если утерян пароль.</li>
  <li>Можно указывать и редактировать личную информацию, менять пароль, эмейл.</li>
  <li>Можно добавлять выплненные работы, изменять все данные в них в том числе и дату,
      если необходимо добавить задачу "задним числом".</li>
  <ul><h5>В статистике за неделю можно увидеть:</h5>
  <li>сколько автомобилей было</li>
  <li>заработок за неделю без вычета процента и заработок с вычтенным процентом который можно указать при регистрации</li>
  <li>самый прибыльный автомобиль, суммарная стоимость по работам за него, и работы которые были выполнены</li>
  <li></li>
  </ul>
  <ul><h5>В статистике за месяц можно увидеть:</h5>
  <li>сколько автомобилей было</li>
  <li>заработок за месяц без вычета процента и заработок с вычтенным процентом</li>
  <li>какие марки автомобилей были и их количество</li>
  <li>суммарное количество выполненных работ</li>
  <li></li>
  </ul>
  </ul>
  <h4>Трудности и выводы</h4>
<p>Т.к. это мой первый относительно большой проэкт и опыта коммерческой разработки у меня нет, не говоря о разработке бэкэнда, трудно было везде.
Было сложно организовать структуру приложения. Как и где должен храниться UI, как хранить action-ы и thunk-и где должен храниться бэкэнд,
как связать фронт с бэком на уровне кода в dev режиме, в prod режиме, 
какую БД использовать и как ее, черт возьми, использовать, я ведь на фронтэнд разарботчика учился и т.д. 
Аренда хостинга, домена, деплой проэкта это все было в новинку и заняло изрядно времени.
</p>
<ul>
Выводы:
  <li>Всегда комментировать код, через неделю забываешь что писал и приходится опять вникать в свою же писанину.</li>
  <li>Писать код без сокращений, никаких вложенных тернарных операторов.</li>
  <li>Коммитить изменения которые относятся только к одной функции/компоненту или группе функций логически связанных между собой.</li>
  <li>Ни в коем случае не разрабатывать логику приложения отталкиваясь от UI. Данные первичны.</li>
  </ul>
  
  <h4>Запуск</h4>
  <ol>
  <li>Клонируем репозиторий</li>
  <li>npm i</li>
  <li>npm run client:install</li>
  <li>npm run dev</li>
</ol>
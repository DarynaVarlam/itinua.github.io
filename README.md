# Добро пожаловать на сайт ITIN.ua социального собирания знаний

12

## Добавления нового материала
Мы расматриваем интересные статьи от всех пользователей.
Интересные статьи, которые относятся к тематике нашего сайта, мы разместим после модерации.
В статье будет имя автора и ссылка на его профиль, с информацией о себе и видам деятельности

## Как добавить новый материал?

## Самое простое, выслать на Email
Вышлите нам на емейл свою статью.
Воспользуйтесь шаблоном:

**Заголок статьи:** например, Вывод денег в Украину  
**Категория:** например, Работа с иностранными компаниями  
**Краткое описание:** например, Помимо принятого сообществом традиционного энциклопедического стандарта на заголовки статей, время от времени у некоторых участников возникают идеи создания своих, искусственных стандартов.  
**Аватор:** Иван Васильев  
**Картинка:** файл или ссылка на илюстарцию к материалу  
__*Сама статья*__
       
Если вы пиште нам первый раз, тогда добавте свое фото, и краткую информацию о себе. 
Например как в разделе [Наши авторы](http://itin.com.ua/content/list/users.html). 
Статья появится на сайте сразу после модерации

## Коллективаная работа с сайтом через GitHub
Миллионы людей совместно работают над статьями и даже целыми ресурсами с помощью [GitHub](https://ru.wikipedia.org/wiki/GitHub).
Внося изменения на GitHub, они появятся у нас на сайте.

**GitHub** самый крупный веб-сервис для хостинга проектов, документов, сайтов и их совместной разработки.
Основан на системе контроля версий [Git](https://ru.wikipedia.org/wiki/Git)

Вот успешне примеры совмесной работы с текстами:  
[Команда математиков за полгода написала 600-страничную книгу, используя GitHub](http://habrahabr.ru/post/184716/)  
[Гражданский кодекс Франции теперь на Github](http://geektimes.ru/post/248196/)  
[Исландия: каждая кухарка может написать Конституцию](http://ttolk.ru/?p=14243)  

## Работа с GitHub
Прочитайте первые разделы книги [Введение в Git](https://git-scm.com/book/ru/v1)  
Зареестрируйтесь на сайте [https://github.com/](https://github.com/)  
Сделайте Fork (Свою копию) нашего проекта [https://github.com/itinua/itinua.github.io](https://github.com/itinua/itinua.github.io)  
Установите Клиент [GitHub on Windows](https://msysgit.github.io/) или [GitHub on Mac](https://mac.github.com/) или [PyCharm](https://www.jetbrains.com/pycharm/)  
Добавте свой репозиторий и сделайте **Синхронизацию**  
**Pull**(тянуть) взять последния изменения  
**Push**(толкать) отдать измения в репозиторий (например правки или новую статью)
Сделайте **Pull Request** в наш репозиторий [itinua.github.io](https://github.com/itinua/itinua.github.io)
  
В дальнейшем, вам неоходимы только три простых действия **Затянуть** последние измения **Толкнуть** свои нам на сайт и попросить их принять.

На самом деле все вышесказанное очень простое действие, так работают миллионы программистов, тестеров, верстальщиков и других образовнных людей.  
В современном мире совместная разработка возможна только благодаря таким вот системам :) 

## Структура сайта

**posts**  В этой папке все статьи   
**content/author** Информация об всех наших авторах  
**images** Картинки к материалам

## Создание новой статьи
Статья появляется автоматически на сайте, когда в нужной папке появляется такой файл.
Например в директории
**_posts/[a1] Работа с иностранными компаниями**

Название файла должно быть в формате  
**2015-06-15**-kak-rabotat-s-google.md  
Где
**2015-06-15** Дата создания или последнего редактирования  
**kak-rabotat-s-google** Название транслитом, потом это будет ссылка URL  
**.md** - формат файла [Markdown](http://webquant.ru/posts/markdown/) или [Детальное описание на Английском](http://daringfireball.net/projects/markdown/syntax)  
Для визуализации вы можете установить один из многих редакторов, например [brackets](http://brackets.io/) (c сплагином Markdown) или например [atom.io](https://atom.io/)

Что бы быстро создать правильное имя файла, воспользуйтель этой формой, например впишите название статьи и нажмите Enter

<script >
    var a = {"Ё":"YO","Й":"I","Ц":"TS","У":"U","К":"K","Е":"E","Н":"N","Г":"G","Ш":"SH","Щ":"SCH","З":"Z","Х":"H","Ъ":"'","ё":"yo","й":"i","ц":"ts","у":"u","к":"k","е":"e","н":"n","г":"g","ш":"sh","щ":"sch","з":"z","х":"h","ъ":"'","Ф":"F","Ы":"I","В":"V","А":"a","П":"P","Р":"R","О":"O","Л":"L","Д":"D","Ж":"ZH","Э":"E","ф":"f","ы":"i","в":"v","а":"a","п":"p","р":"r","о":"o","л":"l","д":"d","ж":"zh","э":"e","Я":"Ya","Ч":"CH","С":"S","М":"M","И":"I","Т":"T","Ь":"","Б":"B","Ю":"YU","я":"ya","ч":"ch","с":"s","м":"m","и":"i","т":"t","ь":"","б":"b","ю":"yu"};
раздела
    function transliterate(word){
    return word.replace(/ь/g, '').replace(/Ь/g, '').split('').map(function (char) {
    return a[char] || char;
    }).join("");
    }
    function onKey(e){
         e = e || window.event;
            if (e.keyCode == 13)
            {

                var text = document.getElementById('btnSearch').value.toLowerCase().replace(/^\s+|\s+$/g,'').replace(/ /g, '-');
                var r = transliterate(text);
                
                var today = new Date().toISOString().slice(0, 10);
                r = today +"-"+ r + ".md";
                document.getElementById('btnSearch').value = r;
                document.getElementById('btnSearch').select();
            }
    }
</script>
###Форма создания имени файла для статьи
<input type="text" id="btnSearch" size="60" onkeypress="onKey(event);"/>  
**Какая система налогообложения мне подходит**
станет  
**2015-06-17-kakaya-sistema-nalogooblozheniya-mne-podhodit.md**  

Это и есть хорошее имя для файла

## Заголовок статьи
В файле статьи обязательно указать заголовок, его можно скопировать с любой статьи нужно раздела  
**---**  
**layout: article** Значит что у нас шаблон статья  
**categories: [a1, actual, featured]** Значит что статья появится в разделе _[a1] Работа с иностранными компаниями_  
  ***actual*** - если статья должна появится внизу в актульных   
  ***featured*** - если статья должна появится как главная, выделенная в разделе  
**title: Как работать с Google** Заголовок   
**about: Бла бла бла** Краткое описание статьи   
**img: money-minimal.jpg** Обязательное имя картинки, картинка долджна находится в папке ***images***   
**author: ivan-ivanenko** Если есть автор  
**---**

И тело статьи

ВСЕ

Создавайте материал и мы его ждем у нас на сайте

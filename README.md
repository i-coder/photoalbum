photoalbum
==========

Демонстрация загрузки картинок

Для загрузки используется плагин jquery.fileUpload, позволяющий загружать файлы различными способами.

Особенности:
* Можно загружать файлы перетаскиванием или обычным способом. По одному или сразу несколько
* Файлы загружаются на сервер, где обрабатываются (если это картинка) и сохраняются в базу
* Результаты обработки картинок складываются в папку с большими изображениями, на которые накладывается копирайт, и миниатюрами
* Описание и порядок расположения картинок сохраняются на сервере
* Большие изображения можно просмотреть в лайтбоксе

__Демонстрация: http://tamtakoe.ru/photoalbum__

Приветствуется любая помощь по дорабоке проекта. В частности:
* Доработать jquery.damnUploader, чтобы его можно было использовать вместо текущего плагина загрузки, т.к. последний чересчур громоздкий. Страница плагина https://github.com/safronizator/damnUploader
* lib/imagick.php - написать плагин для imageMagick, по аналогии с GD и MW
* lib/gd.php, magickwand.php, lib/imagick.php - сделать адаптивное наложение копирайта по типу: http://bravedefender.ru/post133857076/
* jquery.fancybox.js - вырезать всю лишнюю функциональность. Сделать на основе модального окна бутстрапа http://twitter.github.com/bootstrap/javascript.html#modals, поменять анимацию при прокрутке колесом, сделать прокрутку рукой, как в фотораме http://fotoramajs.com/ 
* jquery.damnUploader.js - исправить баг с множественной загрузкой (когда изображения дублируются), разобраться почему скачет прогресс-бар

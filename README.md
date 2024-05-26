# MSA Project 3.2
## Команда
Комаров Олег, Маканин Ярослав, Петелина Полина, Финошина София (БГП201)

## Ссылка
Сайт: https://fobosguy.github.io/msa-project-3.2/ <br />
Docs: https://docs.google.com/document/d/1z2WFV8GwYCacNHzhF3REBbxxRgP7RZSPcAGrWyXDWM0/edit

## Информация
Город Иркутск с населением 606369 человек был основан в 1661 году, расположен в Восточной Сибири, является административным центром Иркутской области.

## Данные
Работа была выполнена на основе главных наборов – полигоны зданий ОКН; административные границы города; прочие ОКН. В общей сложности количество ОКН составило 1090 объектов. Наборы данных были вручную настроены на основе даты, которая была представлена в рамках проекта. Такие данные, как полигоны зданий и административные границы, были взять из OSM.

## Основные методы
Основным методом визуализации стала библиотека Folium. С ее помощью были выполнены базовые задачи проекта по отображению геоданных в интерактивном веб-формате.
Также для одной из фичей была использована библиотека Branca, позволяющая вставлять HTML-код в корень DOM-элемента, формируемого с помощью Folium’a.

## Описание карты
Наша карта представляет все возможные ОКН города Иркутск. В зависимости от масштаба, ближайшие объекты агрегируются в полигоны, которые указывают на количество объектов на части территории. Чем темнее кружок с числом, тем больше ОКН сосредоточено в одном месте. Также на карте визуально представлено сосредоточение памятников посредством цветного грида. У пользователя есть возможность ознакомиться с краткой информацией о памятнике, сделать это можно с помощью нажатия на интересующий объект. Можно заметить, что присутствует несколько вариантов хинтов – обычные и со звездой. С звездой отмечены те ОКН, которые не имеют привязки к зданиям, или иные объекты. 

## Сильные стороны
Одной из интересных возможностей это взаимодействие с легендой, которую можно перетащить и увеличить. Сайт с картой предлагает возможность выбора режима просмотра, например, можно применить к карте dark/light mode, или выбрать, какие элементы будут отображены на карте.

## Сложности
В зависимости от категории памятника здание или хинт (в случае если объект не привязан к зданию) окрашены в определенный цвет. Эта задача стала одной из сложностей проекта, поскольку категории в слоях изначально были атрибутированы с ошибками. Для организации совместной работы проект выполнялся в гитхабе, что стало в какой-то степени челленджем. Можно заметить, что при включении ”Темной темы” легенда “Количество ОКН” перестает быть читаемой, связано это с тем, что у Folium отсутствует встроенный функционал для изменения цвета текста легенды. Также не получилось сделать единую легенду, что влияет на пользовательский опыт. Помимо прочего, не получилось отобразить легенду для категорий ОКН при полноэкранном режиме.

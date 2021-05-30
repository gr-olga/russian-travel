# Проект: Путешествие по России

Описание проекта и его функциональности; одностраничный демонстрационный файл с вертикальной прокруткой, галереями и
описанием. Используются технологии:
HTML5, CCS(flex, grid)

Ссылка на проект: https://gr-olga.github.io/russian-travel/

Комментарий для ревьювера:

Мне не удалось найти хороший способ сделать отступы в промежуточных (между точками перелома) разрешениях экрана. Это
связанно с тем, что я, как вы и сказали, стала использовать `max-width` в сочетании `margin: 0 auto`
и отказалась от отступов (маргины и паддинги по краям элементов).

Проблема следующая, если я задаю `max-width` и `margin: 0 auto` внешнему блоку, то я не могу задать отступы внутреннему
блоку – вёрстка разъезжается (размер блока складывается из `max-width` и отступа). Так же без отступов
вроде `margin-left`, `margin-right` края элементов часто прилепают к краю экрана на промежуточных разрешениях, когда
актуальная ширина экрана становится больше или равна `max-width`. Из-за этого я не вижу иного выхода кроме как добавлять
множество media-query, что мне кажется не очень правильным.

Вопрос в следующем, правильно ли я поступаю, решая эту проблему через media-query? И если нет, то какой тогда правильный
способ решить эту проблему?
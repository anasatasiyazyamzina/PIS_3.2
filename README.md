## Задание 3.2

1. Реализовать запрос на SPARQL с помощью библиотеки SPARQLWrapper.
2. Использовать [https://www.wikidata.org/w/api.php](https://www.wikidata.org/w/api.php).
3. Интегрировать код, реализующий запрос на SPARQL, в код к заданию 2.1 так, чтобы запрос выполнялся для фильмов, полученных в результате работы рекомендующего алгоритма.

Код 3.2: https://github.com/anasatasiyazyamzina/PIS_3.2/blob/main/Zyamzina%203.2%20.ipynb

Задание 2.1: https://github.com/anasatasiyazyamzina/RecSys_2.1.

Вариант в 2.1: 8
Вариант в 3.2: 7

Запрос(7):список фильмов режиссера рекомендованного фильма

Ссылка на запрос в wikiData: https://query.wikidata.org/#%237%3A%20%20список%20фильмов%20режиссера%20рекомендованного%20фильма%0ASELECT%20%3Ffilms%20%3FfilmsLabel%20WHERE%20%7B%0A%20%20wd%3AQ165817%20wdt%3AP57%20%3Fdirector.%0A%20%20%3Ffilms%20wdt%3AP31%20wd%3AQ11424%3B%0A%20%20%20%20wdt%3AP57%20%3Fdirector.%0A%20%20FILTER%28%3Ffilms%20%21%3D%20wd%3AQ165817%29%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cru%22.%20%7D%0A%7D



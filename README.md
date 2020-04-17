# rides-minimal


Текущие задачи:

- [ ] Переносим сюда код из [ноутбука rides2.ipynb на Google Colab](https://colab.research.google.com/drive/1DXsJBTyVvAXrU1aEy5GFWiF_i75LmWS1#scrollTo=h3WG4Nex_pmC)
- [ ] Пишем тесты на основе короткого датасета [one_day.zip](one_day.zip)
- [ ] Генерируем документацию (sphinx, mkdocs-react)
- [ ] Вывешиваем минимальный пример использования пакета на Colab
- [ ] Составляем план/roadmap доработок (вставки из "тяжелого" алгоритма и т.д.)

Псеводкод обработки данных:

- Считали сырые данные из JSON, получили одну таблицу данных
- Упрощение: решили, что будем смотреть путь машины внутри суток без `id_заказа`
- Преобразовали в массив данных в список треков `[Trip]: [поездка:(id_машины, дата), трек:(широта, долгота, метка времени)]`
- Проводим анализ фигур треков в два этапа 
- Получили два коэффициента перекрытия и их сумму для каждой пары треков.
- Сделали выгрузку итоговых треков

<!--

Замысел:

- перетащить сюда код, который мы сделали для "легкой" модели анализа треков
- урезать тестовый датасет до 1 дня - можно писать юнит и end-to-end тесты 
- попутно отрефакторирить код из ноутбука
- документация (sphinx, mkdocs-react)
- привлечь новых коллег к работе над частями кода (отдельные issues)

Выигрыши:

- в ноутбуке будет меньше кода, больше к демонстрации результатов
- можем заняться задачей сближения "тяжелой" и "легкой" модели
- "продуктизация" нашей разработки
- `pip install что-то`
- в целом, лучше подготовимся к последующим работам / развитию проекта

Минусы:

- формально нам не заказывали это сделать, работа подготовительная,
  хотя мы и анонсировали ее
- workflow - не запутаться, кто что делает + это не ноутбук (git + Travis CI)
- у нас не все части в ноутбуке стабильные и полные, надо понимать что там происходит,
  что-то достраивать
  
-->

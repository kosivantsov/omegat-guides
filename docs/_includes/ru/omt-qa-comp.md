## Проверка полного завершения перевода

Все сегменты проекта должны содержать перевод. Перед сдачей выполненной работы надлежит убедиться, что это действительно так.

Для проверки полного завершения перевода наведите указатель мыши на строку состояния в правом нижнем углу главного окна OmegaT.

![](../_img/progress-status.png)

<!-- @todo: red square around the figures -->

В этой панели показана статистика:

- количество переведенных уникальных сегментов (оставшееся количество уникальных сегментов) в текущем файле (например, `100 % (осталось: 0)`, как на снимке экрана выше)

* количество переведенных уникальных сегментов (оставшееся количество уникальных сегментов) в проекте (например, `100 % (осталось: 0)`, как на снимке экрана выше)
* общее количество сегментов (например, `54` как на снимке экрана выше)
<!-- @todo: screenshot with labels showing what is what -->

Если у вас в этой панели показана подобная информация (`100 % (осталось: 0) / 100 % (осталось: 0), 54`), то это означает, что в проекте переведены все 54 сегмента. Если же вы видите, что оставшихся сегментов больше, чем ноль, то перевод проекта не завершен.

При наличии непереведенных сегментов необходимо выполнить следующие действия:

1. Нажмите ++escape++, чтобы закрыть окно **Project Files** (Файлы проекта).
2. Нажмите сочетание клавиш ++ctrl+u++, чтобы перейти к **следующему непереведенному сегменту**.
3. Переведите сегмент.

Повторяйте описанные выше действия до тех пока, пока в проекте не останется непереведенных сегментов.

Наконец, еще раз проверьте строку состояния, чтобы подтвердить завершение перевода.

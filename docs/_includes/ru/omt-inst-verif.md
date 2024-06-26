# Руководство по установке OmegaT 5.7.2 для Windows

<!-- prettier-ignore -->
??? info "Другие операционные системы"
    Программ OmegaT может быть установлена на другие операционные системы, такие как macOS или Linux. Установка на macOS описана в [этом руководстве](install-and-setup-macos.md). Если требуется установка на Linux, свяжитесь с нашей службой поддержки.

Вам следует ==тщательно выбрать правильный вариант==, исходя из своих начальных условий:

- Если у вас уже установлена предыдущая версия OmegaT (например, 5.7.1 или 4.2.0), вам следует сначала обновить конфигурацию программы. Как это сделать, описано в [разделе о конфигурации](#configuration) (следующий раздел).
- Если на вашем компьютере ранее _никогда_ не была установлена OmegaT (любой версии), то вы можете пропустить следующий раздел, посвященный конфигурации программы, и перейти непосредственно к [разделу об установке](#installation). OmegaT будет сконфигурирована автоматически в процессе установки.

## Конфигурация

Этот раздел предназначен для пользователей, на компьютере которых уже установленна предыдущая версия OmegaT (например, 5.7.1 или 4.2.0). Для обновления конфигурации программы выполните шаги, приведенные ниже.

1. Запустите OmegaT и перейдите в меню **Tools** (Инструменты) > **Scripting** (Скрипты), чтобы открыть консоль скриптов. В OmegaT 5.7.1 откройте консоль скриптов. Проверьте, есть ли у вас скрипт под названием **Update Customisation Bundle (v572)**:

   <!-- prettier-ignore -->
!!! warning "Предупреждение"
       Если в названии нет фрагмента «**v572**», то это не тот скрипт, который нам нужен. В следующем шаге описано, где взять этот скрипт.

   ![](../_img/custom-script-572-in-scripting-console.png)

   Если скрипт **Update Customisation Bundle (v572)** есть в списке, выберите его щелчком мыши и нажмите кнопку **Run** (Выполнить) в левом нижнем углу окна для запуска скрипта. Скрипт выполнит обновление файлов конфигурации и завершит работу OmegaT. Далее пропустите следующий шаг и перейдите непосредственно к [разделу установки](#installation).

   Если скрипт отсутствует в списке, вы можете скачать его самостоятельно. В дальнейших шагах описано, как это сделать.

2. Нажмите правой кнопкой мыши на кнопку ниже и выберите «Сохранить как», чтобы загрузить скрипт конфигурации (например, на рабочий стол)7

   [:material-download: Скачать UpdateConfigBundle.groovy](https://cat.capstan.be/OmegaT/customization/scripts/updateConfigBundle-572.groovy){ .md-button .md-button--primary }

3. В главном окне OmegaT выполните следующие действия для запуска скаченного скрипта конфигурации:

   - **Tools** (Инструменты) > **Scripting** (Скрипты) > **File** (Файл) > **Open script** (Открыть скрипт).
   - Перейдите на рабочий стол (или в папку, в которой был сохранен скрипт) и выберите файл с расширением groovy.
   - Нажмите кнопку **Open** (Открыть), чтобы открыть файл скрипта, далее нажмите кнопку **Run** (Выполнить)в левом нижнем углу окна.

   ![](../_img/omt-open-script-and-run.gif)

   Скрипт установит необходимые файлы конфигурации для OmegaT 5.7.2 и удалит старые файлы для предыдущих версий, после чего завершит работу программы.

4. Удалите текущую версию OmegaT.

5. После этого переходите к [разделу установки](#installation) (следующий шаг).

## Установка

<!-- prettier-ignore -->
!!! warning "Предупреждение"
    Для установки OmegaT необходим 64-разрядный компьютер.

1. Нажмите на кнопку ниже, чтобы загрузить OmegaT 5.7.2. Это специальная версия, подготовленная компанией cApStAn. Она включает в себя несколько исправлений ошибок и улучшений, недоступных в других версиях.

   [:material-download: Загрузить OmegaT 5.7.2](https://cat.capstan.be/OmegaT/exe/OmegaT_5.7.2_Windows_64_Signed.exe){ .md-button .md-button--primary }

   <!-- prettier-ignore -->
??? question "Проблемы с загрузкой?"
       В некоторых браузерах (например, в Microsoft Edge) может появиться диалоговое окно с вопросом о безопасности загрузки установочного файла. Файл безопасен. Чтобы разрешить загрузку файла в браузере, вы можете выполнить действия, показанные в следующем видео.

   ![](../_img/edge-keep-download.gif)

2. После завершения загрузки дважды щелкните установочный файл, чтобы запустить мастер установки.

3. Windows Defender (Центр защиты Windows) может показать предупреждение о риске запуска неизвестного приложения.

   ![](../_img/omegat-win-protected-your-pc-01.png)<!-- # omt572-install-01.png -->

   При появлении такого диалогового окна щелкните ссылку <u>More info</u> (Подробнее). В появившемся окне вы должны увидеть информацию о том, что издателем этой программы установки является cApStAn.

   ![](../_img/omt572-install-02-run-anyway.png)

   Если это действительно так, нажмите кнопку **Run anyway** (Выполнить в любом случае) для продолжения установки.

4. В следующем диалоговом окне можно выбрать язык установки. Далее нажмите **OK**:

   ![](../_img/omt572-install-03-lang.png)

5. Чтобы продолжить установку, примите лицензионное лицензионное соглашение GPL и нажмите **Next** (Далее):

   ![](../_img/omt572-install-04-accept.png)

6. В процессе установки будет предложено установить программу OmegaT в папку `C:\Users\USER\AppData\Local\Programs\OmegaT`. Такой выбор пути установки позволяет установить программу пользователям без административных прав.

   <!-- prettier-ignore -->
!!! warning "Предупреждение"
       Не изменяйте путь установки, если вы не являетесь ИТ-специалистом и не знаете, что делаете.

   ![](../_img/omt572-install-05-path.png)

7. На рабочем столе будет создан ярлык, благодаря которому впоследствии можно запускать OmegaT двойным щелчком. Оставьте эту опцию включенной.

   ![](../_img/omt572-install-06-desktop-shortcut.png)

8. Вы можете изменить название папки OmegaT в меню «Пуск», но предложенное название «OmegaT» вполне подходить, при стандартной установке его менять не нужно.

   ![](../_img/omt572-install-07-start-menu.png)

9. Теперь вы можете приступить к установке. Нажмите кнопку **Next** (Далее).

   ![](../_img/omt572-install-08-ready.png)

10. Установка должна завершиться через несколько минут.

   ![](../_img/omt572-install-09-done.png)

11. В следующем разделе вы узнаете, как после установки выполнить несколько проверок, чтобы убедиться, что все в порядке.

Все готово. Можно приступать к использованию OmegaT 5.7.2.

## Проверка надлежащей установки

Описанные выше действия, как правило, приводят к успешной установке и запуску OmegaT, но на всякий случай бывает полезно проверить, все ли в порядке.  Проверить можно следующее:

1. _Версия OmegaT_

   Чтобы подтвердить, что у вас действительно установлена правильная версия, вы можете проверить информацию в меню **Help** (Справка) > **About** (О программе) > **Copy Support Info** (Копировать информацию для поддержки). Вы должны увидеть:

       > Version: OmegaT-5.7.2_0_a978d82ee
       > Platform: [ваша операционная система]
       > Java: 11.0.19 amd64

2. _Версия пользовательской конфигурации_

   Чтобы убедиться в том, что ваша пользовательская конфигурация актуальна, можно выбрать пункт меню **Options** (Параметры) > **Access Configuration Folder** (Открыть папку настроек) и найти в открывшейся папке файл под названием `local_version_notes.txt`.

   Если вы откроете этот файл, строка в начале файла, показывающая самое последнее обновление, должна совпадать с той, которую можно увидеть на странице [https://cat.capstan.be/OmegaT/v572/](https://cat.capstan.be/OmegaT/v572/).

3. _Пункты меню распаковки/упаковки OMT_

   Даже если вы не используете пакеты OMT, у вас должно быть три пункта в меню **Project** (Проект) в OmegaT:

   ![](../_img/omt-package-entries.png)

   <!-- - Unpack project from OMT file...
       - Pack project as OMT file...
       - Pack and delete project...  -->

4. _Скрипты и сочетания клавиш для запуска скриптов_

   В меню **Tools** (Инструменты), под пунктом **Scripting** (Скрипты), вы должны увидеть перечень из 12 сочетаний клавиш для запуска скриптов.

   ![](../_img/omt-scripts-shortcuts.png)

!!! note "Примечание"
       Время от времени перечень и сочетания могут обновляться, и если ваш список не совпадает со снимком экрана, не стоит волноваться.

   Кроме того, если вы откроете окно со скриптами, то увидите весь список доступных скриптов в левой части окна.

<!--
To install OmegaT and set it up on a computer running Windows, please follow the OmegaT installation and setup guide below:

<div style="width: 100%">

<iframe
src="https://slides.com/capstan/omegat-v572-setup-guide/embed?byline=hidden&share=hidden"
width="100%"
height="420"
scrolling="no"
frameborder="0"
webkitallowfullscreen mozallowfullscreen allowfullscreen>
</iframe>

</div>

If you use Mac or Linux, please see the second slide above or get in touch through the Helpdesk.


- USB
16GBc
model...
format as FAT32
D:\OmegaT
zip -- iso


https://www.westerndigital.com/products/usb-flash-drives/sandisk-ultra-fit-usb-3-1?sku=SDCZ430-016G-G46

-->

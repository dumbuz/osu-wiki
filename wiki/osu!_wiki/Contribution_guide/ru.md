# Руководство по работе с osu! wiki

Спасибо за интерес, проявленный к osu! wiki. В этой статье вы найдёте подробное описание того, как редактировать вики. Если вы знакомы с GitHub, пользуйтесь схемой «одна статья (или группа статей на одну тематику) — одна ветка», а потом сразу переходите к разделу «[Самопроверка](#самопроверка)».

От новых редакторов не ожидается знание GitHub или [git](https://git-scm.com/), так как эти инструменты в основном применяются разработчиками. Если что-то пойдёт не так, не переживайте: кто-нибудь из [администраторов osu! wiki](/wiki/People/osu!_wiki_maintainers) либо поможет советом, либо самостоятельно исправит проблему.

Если вам в какой-то момент понадобится помощь, обращайтесь в [дискорд-сервер osu!dev](https://discord.gg/ppy) на канал `#osu-wiki`.

## Чем можно помочь

Если у вас есть желание помочь, но нет понимания, с чем именно, загляните в раздел [Работа над osu! wiki § Рутинные задачи](/wiki/osu!_wiki/Maintenance#рутинная-работа). В ней описаны задачи, которые нуждаются в регулярном контроле, и прочие способы помочь. Если вы пытаетесь понять, как тут работает форматирование, посмотрите [шпаргалку по Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Редактирование вики

*О том, как в целом устроен процесс внесения правок в чужие репозитории, см. [GitHub flow - GitHub Docs](https://docs.github.com/en/get-started/quickstart/github-flow)*

Статьи osu! wiki хранятся на [GitHub][osu_wiki]. Чтобы их отредактировать, нужно сделать следующее:

0. [Зарегистрируйтесь](https://github.com/signup) на GitHub.
1. Откройте репозиторий [`ppy/osu-wiki`][osu_wiki] и нажмите на кнопку с подписью `Fork`, которая находится в правом верхнем углу. Так вы создадите копию osu! wiki, к которой будете иметь полный доступ. Чтобы по-быстрому перейти к копии, откройте [`ppy/osu-wiki`][osu_wiki] и снова нажмите на кнопку `Fork`.

  - Если у вас уже есть форк, его необходимо [синхронизировать](/wiki/osu!_wiki/Contribution_guide/Best_practices#как-синхронизировать-форк).

2. Внимательно прочитайте раздел [Как правильно работать с вики § Внесение правок](/wiki/osu!_wiki/Contribution_guide/Best_practices#внесение-правок) и сделайте нужные изменения в форке (переведите статью, добавьте картинки и т.д.) – для этого можно пользоваться любыми доступными программами и инструментами. На osu! wiki есть инструкции к двум наиболее популярным из них:

  - [Веб-редактор GitHub](/wiki/osu!_wiki/Contribution_guide/GitHub_web-based_editor) (браузерное приложение, не требует установки).
  - [GitHub Desktop](/wiki/osu!_wiki/Contribution_guide/GitHub_Desktop) (обычное приложение, имеет больше возможностей).

## Самопроверка

Потратьте несколько минут на то, чтобы проверить свои изменения по списку ниже:

- **Стиль письма**: статьи osu! wiki, за редким исключением, должны быть написаны нейтрально.
- **Содержание и правописание**: статьи должны быть написаны внятным и доходчивым языком, а также не вгонять читателя в ступор своими формулировками. Будьте последовательны при изложении мыслей и избегайте переусложнённых или обрывистых предложений: вы пишете для живых людей. По возможности пользуйтесь редакторами со встроенной проверкой орфографии и пунктуации, чтобы отлавливать ошибки и опечатки (например, [Google Docs](https://docs.google.com)).
- **[Равенство содержания](/wiki/Article_styling_criteria/Writing#равенство-содержания)**: в переводах должна содержаться та же информация, что и в оригиналах (само собой, допускаются расхождения в формулировках или пунктуации). Если вам кажется, что в оригинальной статье не хватает чего-то важного, или она устарела, не пытайтесь улучшать перевод «на ходу» — [заведите issue](https://github.com/ppy/osu-wiki/issues/new) или отправьте пулл-реквест с оригинальными правками, если хватает времени или сил.
- **Структура и оформление**: чтобы проверить форматирование, откройте статью в каком-нибудь редакторе, умеющем показывать превью, например, [Markdown Editor от jbt](https://jbt.github.io/markdown-editor/).
- **Изображения и прочие бинарные файлы** должны «весить» [меньше одного мегабайта](/wiki/Article_styling_criteria/Formatting#размер-файла). **Скриншоты** нужно делать с выбранным стандартным скином и [некоторыми настройками](/wiki/Article_styling_criteria/Formatting#скриншоты-игрового-процесса), например, в разрешении 1280×720.

Полный список правил есть в [критериях оформления статей](/wiki/Article_styling_criteria). Критерии не нужно заучивать; достаточно бегло их просмотреть, а на упущенные ошибки вам укажут при ревью.

## Пулл-реквест

Если вы перепроверили свою работу, закоммитили и запушили все правки, их теперь нужно показать администраторам osu! wiki. Это делается с помощью отправки пулл-реквеста:

1. Откройте **ваш форк** osu! wiki, найдите кнопку с надписью `master↓` и выберите там ветку с нужными изменениями.
2. Нажмите на кнопку `Contribute↓` и выберите пункт `Open pull request`.
3. Прочитайте [Как правильно работать с вики § Как отправить пулл-реквест](/wiki/osu!_wiki/Contribution_guide/Best_practices#как-отправить-пулл-реквест) и заполните текстовое поле. После этого нажмите на кнопку `Create pull request`.

## Ревью

Все правки проверяются. На практике это означает, что другие люди будут читать ваш пулл-реквест, искать в нём ошибки и описывать или напрямую предлагать варианты исправлений. Во время ревью, как это везде принято, необходимо реагировать на замечания: их нужно либо [исправлять](/wiki/osu!_wiki/Contribution_guide/Best_practices#как-применять-ревью), либо объяснять, почему вы не хотите так поступать.

Если к вам никто не заглянул, а время идёт, попробуйте что-нибудь сделать:

- Убедитесь, что вы разобрались со всеми замечаниями. Возможно, кто-то из текущих или будущих ревьюеров ждёт именно этого.
- Загляните на канал `#osu-wiki` в [дискорд-сервере osu!dev](/wiki/Community/osu!dev_Discord_server) и попросите там о ревью, либо оставьте комментарий к своему пулл-реквесту.
- Чтобы понять, у кого искать помощи с русским языком, посмотрите чужие переводы и свяжитесь либо с их авторами, либо с ревьюерами ([ссылка для поиска русских переводов на GitHub](https://github.com/ppy/osu-wiki/pulls?q=is%3Apr+is%3Amerged+%5BRU%5D)).
- Если у вас есть друзья, хорошо знающие язык или разбирающиеся в предмете, обратитесь к ним!

Помимо процесса ревью, в репозитории osu! wiki есть [автоматические проверки](/wiki/osu!_wiki/Maintenance#автоматизированные-проверки), контролирующие оформление статей. Чтобы посмотреть, как они отработали, откройте пулл-реквест и перейдите на вкладку `Actions` – если там есть ошибки, в них будет написано, что и где именно нужно исправить.

## Публикация

Рано или поздно ваш пулл-реквест проверит один из [администраторов вики](/wiki/People/osu!_wiki_maintainers) – обычно это происходит после ревью от других людей. Если ничего не происходит в течение нескольких дней, позовите администраторов в комментариях к пулл-реквесту, либо на канале `#osu-wiki` в [дискорд-сервере osu!dev](/wiki/Community/osu!dev_Discord_server). После того, как вашу ветку вольют в `master`, соответствующие статьи обновятся (чаще всего это происходит за пару секунд, в худшем случае – в течение пяти часов).

[osu_wiki]: https://github.com/ppy/osu-wiki

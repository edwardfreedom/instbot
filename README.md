# UPD: Используйте GUI, этот репозиторий стал внешним модулем.
[d0kur0/instBotGui](https://github.com/d0kur0/instBotGui)

# Instbot

![Процесс работы програмы](https://pp.userapi.com/c851216/v851216067/de22f/XDfyb98BiG4.jpg)

Instbot - бот для instagram, написанный на JavaScript c использованием headless браузера [Pupetteer](https://github.com/GoogleChrome/puppeteer).

Функционал бота крайне прост. Он берёт страницу нужного хештега или локации (перечисленных в файле конфигурации) и перебирает все посты по порядку, ставит лайк, подписывается на автора поста и пишет комментарий из словаря (рандомный). Время от времени меняет открытый хештег/локацию. Есть поддержка ограничений в виде дневных лимитов на подписки, лайки и комментарии (чтобы не отлететь в бан), можно вручную проставлять паузы между действиями.

Функции разделены на модули и каждая из них включается и отключается по-отдельности.
Целевая идея в том, что люди создают ответный трафик, подписываются и лайкают посты того, от кого был запущен бот. При этом не требуя какх либо затрат.

**Время от времени инстаграм обновляется и может ломать бота, я по возможности и желанию обновляю его.
Если Вам нужна срочная помощь в запуске бота, требуеутся разработать какую-то дополнительную фичу - пишите на почту или в телеграмм (@liaFcipE), но сразу скажу, что это не будет бесплатным.**

## Что требуется?
NodeJS 14+ version.

## Как использовать?

Клонируешь или качаешь репозиторий, в папке ```app``` есть файл ```settings.json-example```, копируешь его как ```settings.json``` (ну или просто переименовываешь).
Открываешь этот файл и заполняешь его, все поля в принципе интуитивно понятны, если что-то не понятно - лучше скачай GUI версию, там всё описано.

### Запуск
Всё просто, достаточно из корня проекта сделать: ```node --experimental-json-modules app/index.js```, параметр для включения JSON модулей обязателен, без него работать не будет, когда-то он выйдет из под флага, но пока только так.

Удачи.

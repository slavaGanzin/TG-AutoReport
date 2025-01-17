# TG-AutoReport

Перша версія програми для автоскарг на сепаратиські канали в телеграмі.

❗️ Якщо виникає якась помилка - не соромтесь створювати [ISSUE](https://github.com/NoImN0t/TG-AutoReport/issues) і
присилати текст помилки або знімок з екрана.

Програма написана в навчальних цілях і не може бути використана для злодіянь!
Ми не несемо відповідальності за ймовірне неправильне використання програми!

Використовується мова програмування Python і бібліотека Pyrogram.

У файлі .env ми надаємо вам свої `api_id` і `api_hash`. Згодом вони можуть бути заблоковані, тому їх прийдеться замінити
на свої з сайту https://my.telegram.org

У файлі ban_channels.txt знаходяться канали, на які бот буде скаржитись. Просимо вказувати канали тільки у вигляді "
@channel", інакше працездатність не гарантована.

❗️ Пізніше програму буде оновлено і вона сама буде отримувати актуальні посилання на канали для скарг. Слідкуйте за
репозиторієм.

## docker
```
  sudo docker run -ti --rm slavaganzin/tgautoreport @mardanaka t.me/akashevarova superdolgov
```


## Є 2 способи запуску програми:

### Перший спосіб:

	Якщо ви не розумієте мову програмування Python - то вам потрібно:
        1. Завантажити Python версії 3.8.* або 3.9.* або 3.10.* і вище, де зірочка це люба цифра
        2. Встановити його (не забудьте поставити галочку на пункт 'Add in PATH').
        3. Запустити файл 'start_bot.bat'
        4. Слідувати інструкціям

    Програма попросить у вас номер телефону, на який зареєстровано телеграм.
    Це може бути також віртуальний номер телефону, головне щоб на ньому вже був зареєстрований аккаунт!
		
    Після того як ви ввели номер телефону - у вас попросять код, який прийде вам в телеграмі.
		
    [Опціонально] - Також можуть попросити ввести пароль від двофакторної авторизації.
		
    Після введення всіх даних програма закриється і збереже конфігурацію.
    Повинен створитись файл 'session'.
	
	❗️❗️❗️ УВАГА: НЕ НАДСИЛАЙТЕ НІКОМУ І НЕ ПУБЛІКУЙТЕ ФАЙЛ 'session'!!!
	❗️❗️❗️ ЦЕ ВАШ КЛЮЧ ВІД АККАУНТУ!!!

    Далі просто запустіть програму знову і вона попросить вас ввести команду /report в чат 'Збережене' або 'Избрнанное'.
    (Програма надішле вам повідомлення в цей чат)
		
    Після введення команди - почнеться процесс надання скарг на канали.
		
    ❗️❗️❗️ Будьте обережні і не скаржіться більше чим на 30-40 каналів на день
		
    Щоб зупинити програму - просто закрийте вікно.

### Другий спосіб:

	Якщо ви розумієте мову програмування Python - то ви можете дослідити код у файлі `main.py`
	Ви можете змінити конфігурацію кода і сам код як вам завгодно.
	Тільки одне прохання - не змінювати версію '__version__'!

    Обов'язково інсталюйте бібліотеки з requirements.txt
	
	Надалі ви можете запустити програму для багатьох акаунтів.

Будьте обережні, ваш акаунт можуть заблокувати за надмірну активність. Якщо це трапилось - пишіть
на https://telegram.org/support

Ми не збираємо ніяку інформацію!
Ви можете дослідити код і впевнитись в цьому!

Звісно ви все робите на свій страх і ризик!

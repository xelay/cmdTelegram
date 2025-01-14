# Design Specification

## Экран входа и аутентификации
•	Появляется при запуске приложения.
•	Запрашивает у пользователя телефонный номер и отображает поле для ввода кода подтверждения (получаемого по SMS).
•	После успешного входа перенаправляет пользователя на основной экран.
## Основной экран (со списком чатов)
•	Содержит список всех доступных чатов (личных, групповых и каналов).
•	Отображает активные чаты с указанием количества непрочитанных сообщений.
•	Обозначение новых сообщений (выделение цветом или символами).
•	Навигация по списку — стрелки вверх/вниз. Для выбора чата — Enter.
## Экран чата
•	Отображает историю сообщений выбранного чата.
•	В верхней части экрана указывается название чата и текущий статус пользователя (в сети/не в сети).
•	В нижней части — поле для ввода сообщения.
•	Клавиша Enter отправляет сообщение, клавиша Esc возвращает на главный экран.
•	Возможность просмотра вложений и медиа, доступных для отображения в текстовом формате.
<pre>
╔═══════════════════════════════════════════════════════════════════════════════════════════════╗
║ Telegram Client                                                                               ║
╠════════════════╦══════════════════════════════════════════════════════════════════════════════╣
║                ║                                                                              ║
║    ЧАТЫ        ║       Активный чат: [Название чата]                                          ║
║                ╠──────────────────────────────────────────────────────────────────────────────╣
║    > Чат 1     ║  12:05  Пользователь1: Привет!                                               ║
║      Чат 2     ║  12:06  Пользователь2: Привет, как дела?                                     ║
║      Чат 3     ║                                                                              ║
║      Чат 4     ║  12:07  Пользователь1: Всё отлично!                                          ║
║      Чат 5     ║                                                                              ║
║      Чат 6     ║  12:08  Пользователь2: Отлично! Как продвигается проект?                     ║
║      Чат 7     ║                                                                              ║
║      Чат 8     ║                                                                              ║
║      Чат 9     ║                                                                              ║
║      Чат 10    ║  -- конец сообщений --                                                       ║
║                ║                                                                              ║
║                ╠──────────────────────────────────────────────────────────────────────────────╣
║                ║ Введите сообщение:                                                           ║
║                ║ >                                                                            ║
║                ╠──────────────────────────────────────────────────────────────────────────────╣
║                ║ Навигация: ↑ ↓ для перемещения по списку чатов, Enter для выбора чата,ESC для║
║                ║ выхода, Tab для перехода в область ввода                                     ║
╚════════════════╩══════════════════════════════════════════════════════════════════════════════╝
</pre>



## Экран профиля пользователя и настроек
•	Отображает основные сведения о текущем пользователе: имя, телефон, статус.
•	Настройки, доступные в текстовом формате: уведомления, автообновления и кэш сообщений.
•	Возможность выйти из аккаунта и завершить текущую сессию.

Пожалуйста, прочитайте инструкцию до конца!
Данный скрипт совместим с Debian, Ubuntu и на них основанных и требует работы от имени root

Загрузите скрипт: 
```curl -O https://raw.githubusercontent.com/dementr0n/Hikka-autoinst/master/hikka_autoinst_root.sh && sudo chmod +x hikka_autoinst_root.sh && sudo ./hikka_autoinst_root.sh```


После завершения работы скрипта юзербот попросит вас ввести API ID, API Hash(вы можете получить их на my.telegram.org), на вопросе о QR нажмите Enter, введите номер телефона, код подтверждения и пароль(если установлен) и ждите ±10 минут, зависит от ресурсов хоста.

Для корректной работы автозапуска вам необходимо загрузить модуль systemd (.dlm systemd), написать команды:

1: .addunit hikka

2: .units

3: Нажать на единственную кнопку hikka, и нажать Start для запуска юнита systemd.

4: Написать команду .terminal reboot

Скрипт конфигурирует systemd юнит, который автоматически запускает и перезапускает юзербота, системы с OpenRC(например Alpine)/SystemV(Devuan) НЕ ПОДДЕРЖИВАЮТСЯ!

Благодарности: github.com/hikariatama за юзербота Hikka.

О любых неполадках в работе скрипта сообщайте тут через Issues

P.S. Если вы хотите установить юзербота версии 1.6.4(Без надобности НЕ устанавливайте 1.6.4, она нестабильна и несет риск аккаунту), используйте команду:
.terminal git fetch && git checkout v1.6.4 && git pull

# NavTALink

Модифицированный программно-аппаратный комплекс [DuoCam](duocam.md) с Wi-Fi-адаптером на базе микросхемы **rtl8812au** предназачен для передачи видео и телеметрии между БПЛА и наземной станцией управления на большие расстояния.

## Технические характеристики (TODO)

## Образ NavTALink

Образ предназначен для работы с **Raspberry Pi 4** и базируется на **Raspbian Buster**.

Для связи "БПЛА-станция наземного управления" успользуется трансивер UDP-пакетов через кадры 802.11 [wifibroadcast](https://github.com/svpcom/wifibroadcast).

Также в образе включен:

1. Драйвер [rtl8812au](https://github.com/aircrack-ng/rtl8812au.git) версии **v5.2.20**.
2. Мост для передачи MAVLink сообщений из последовательного порта в UDP [mavlink-serial-bridge](https://github.com/CopterExpress/mavlink-serial-bridge.git).
3. MAVLink-коммутатор [mavlink-fast-switch](https://github.com/CopterExpress/mavlink-fast-switch.git).
4. Программная часть комплекса [DuoCam](duocam.md) и его зависимости.

[Инструкция по настройке комплекса.](navtalink_setup.md)

# ROI - Region Of Interest

Работа с точками интереса с прошивкой PX4 в приложении QGroundControl

## Настройка полетного контроллера

В данный момент на версиях прошивок 1.8.* - 1.9.* ROI по умолчанию не работают, сейчас они корректно работают только на кастомных прошивках COEX:

В ветках:

* [strict_precland+flirduo+video_waypoints+flow](https://github.com/CopterExpress/Firmware/tree/strict_precland+flirduo+video_waypoints+flow)
* [strict_precland+flirduo+video_waypoints](https://github.com/CopterExpress/Firmware/tree/strict_precland+flirduo+video_waypoints)

По тегам:

* [v1.8.0-duocam_flow.1](https://github.com/CopterExpress/Firmware/tree/v1.8.0-duocam_flow.1)
* [v1.8.0-duocam_flow.2](https://github.com/CopterExpress/Firmware/tree/v1.8.0-duocam_flow.2)

При использовании этих веток есть свои нюансы. Для того, что бы точка ROI корректно передавала свои lat, lon координаты, требуется записывать миссию на внутреннюю RAM полетного контроллера. Для этого требуется изменить параметры запуска утилиты dataman отвечающей за работу с миссиями. Это можно сделать двумя путями:

> **Caution** В отличие от записи миссии на SD карту, в случае, когда вы используете RAM, при каждой перезагрузке полетного контроллера, записанная миссия будет стираться. Всегда имейте сохраненный файл миссии для того, что бы разработанный вами полетный план не был утерян.

1. Ручной перезапуск dataman'а с параметром записи на RAM
    Для этого в MAVLink консоли требуется остановить dataman, а потом перезапустить его с флагом *-r*:

    ```bash
    dataman stop
    dataman start -r
    ```

2. Изменение прошивки для автоматической установки RAM как главного хранилища миссии
    В таком случае потребуется вручную менять исходные файлы прошивки и пересобирать ее вручную. Требуется сделать 2 изменения:

    * В файле ROMFS/px4fmu_common/init.d/rcS:
        Изменить строку `set DATAMAN_OPT ""` на `set DATAMAN_OPT -r`
    * В файле src/modules/navigator/navigation.h:
        Перед строкой `#if defined(MEMORY_CONSTRAINED_SYSTEM)` добавить `#define MEMORY_CONSTRAINED_SYSTEM`

В случае настройки dataman'а первым способом нужно учитывать, что объем внутренней RAM ограничен и количество возможных точек миссии соответственно меньше, чем в случае записи на SD карту. Во втором случае предел размера миссии будет жестко заданным и будет равняться 50, в случае если количество точек миссии будет превышать 50, будет возникать ошибка и миссия не будет записана.

Также для работы с ROI нужно установить параметр `MIS_MNT_YAW_CTL` в значение *Disable*.

## Работа с ROI в QGroundControl

Для использования ROI в полетной миссии вам нужно добавить ее после той точки, после которой нужно будет начать доворачивать нос коптера.

Инструкция:

1. Во вкладке *Category* выберете параметр *Camera*
2. В появившемся меню выберете требуемую позицию *Region of interest (ROI)*, если нужно установить точку интереса или *Cancel ROI*, если вам нужно отключить доворот угла

    ![Установка точки ROI](img/roi_mission.png)

3. На карте перетащите появившуюся точку в место, на которую должен доворачивать нос коптер

    ![ROI в миссии](img/mission_setup.png)
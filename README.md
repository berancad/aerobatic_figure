# Реализация фигуры высшего пилотажа на lua скрипте под Ardupilot

Реализованы две акробатические фигуры пилотажа (условные названия "S петля Иммельмана" и "квадратная петля") с использованием библиотеки plane_aerobatics (доступна по ссылке https://github.com/ArduPilot/ardupilot/blob/master/libraries/AP_Scripting/applets/Aerobatics/FixedWing/plane_aerobatics.lua )

Установка:

1. Устанавливаем Mission Planner
2. Запускаем SITL для самолета (выбираем модель plane-3d)
3. Включаем использование скриптов (параметр SCR_ENABLE = 1)
4. Копируем файлы plane_aerobatics.lua и trick77.txt в папку scripts
5. Перезапускаем скрипты в контроллере
6. Формируем полетное задание (выбираем высоту не менее 200 м), одной из точек ставим тип SCRIPT_TIME со значением параметра 77
7. Взлетаем (режим TAKEOFF и ARM)
8. Стартуем миссию (Mission start)
9. После завершения миссии нажимаем DISCONNECT для получения логов

Для удобного (и более красочного) просмотра фигур пилотажа из логов можно использовать сервис https://www.flightcoach.org/ribbon/plotter.html (нужно загрузить соответствующий BIN файл из папки logs в Mission Planner)

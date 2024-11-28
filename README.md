**МОДУЛЬ А**

Присвоенное имя робота в сети:
```
turtlebroXX    
```
IР-адрес робота в сети роутера-полигона:
```
192.168.1.XX
```
Текущая частота подключения робота к сети 5 ГГц:
```
iwconfig
```
Скорость передачи данных через сетевой интерфейс робота(Мбит/с):
```
iperf3 -c 192.168.1.XX
```
Название дистрибутива и кодовое имя сборки Linux:
```
lsb_release -a
```
Версия интерпретатора Python3:
```
python3 -V
```
Версия библиотеки rospy:
```
rosversion rospy
```
Версия библиотеки turtlebro:
```
rosversion turtlebro
```
Версия прошивки микроконтроллера материнской платы и серийный номер системной платы робота:
```
rosservice call /board_info {}
```
Размер оперативной памяти (Мбайт):
```
free -m
```
Текущий часовой пояс на роботе в формате "Time
zone:Continent/City (XXX, +XXXX)":
```
timedatectl|grep "Time zone"
```
Серийный номер Raspberry Pi 4:
```
cat /sys/firmware/devicetree/base/serial-number
```
Топики из инструкции к роботу присутствуют на роботе:
```
rostopic list
```
Температура процессора в градусах (С):
```
vcgencmd measure_temp
```
Текущее разрешение камеры(пикселей):
```
rostopic echo /camera/image_raw
```
Значение напряжения аккумуляторной сборки из топика батареи:
```
```
IMU датчик работает корректно:
```
```
Лидар работает корректно:
```
```
Стерео-акустическая система работает корректно:
```
```
Датчик тепловизор работает корректно:
```
```
Концевой выключатель работает корректно:
```
```
Светодиодная подсветка работает корректно:
```
```
Кнопки  D22-25 работают:
```
```
Связь контроллера расширения с ROS работает:
```
```
**МОДУЛЬ Б**
```
grep "ошибка" master.log > error message.txt
```
b2.2
```
from datetime import datetime
def counter(time1, time2, times_format="%H:%M:%S"):
    a1 = datetime.strptime(time1, times_format)
    a2 = datetime.strptime(time2, times_format)
    b = a2 - a1
    return b
time1 = "times"
time2 = "times"
c = counter(time1,time2)
print("Разница во времени:",с)
```

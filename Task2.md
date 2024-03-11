# Задание 2: Вакуумная граната!

## Описание

В этом задании мы реализуем механику вакуумной гранаты. Эта граната будет притягивать к себе всех врагов, которые попали в радиус взрыва и постепенно уменьшать их размер до нуля. После определенного времени все затянутые враги уничтожаются.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/task2.gif" width="600"/>

## Инструкция

1) Для начала создадим скрипт гранаты [VacuumGrenade.cs](https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/scripts/VacuumGrenade.cs)

Внимательно изучи скрипт, замени ??? на правильные фрагменты кода

Создай префаб гранаты

Он будет состоять из трех осноных частей.

1) Верхнеуровневый пустой объект VacuumGrenade. Добавь в этот объект компонент Rigidbody и скрипт VacuumGrenade. Настрой параметры гранаты.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/VacuumGrenade.png" width="600"/>

2) Визуальная сфера взрыва. Создай объект сферу внутри VacuumGrenade и назови ее Explosion. Удали у сферы коллайдер. Выключи этот объект, чтобы граната появлялась сначала без сферы взрыва.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/VisualExplosion.png" width="600"/>

Навесь на сферу материал с параметром Fade. Настрой цвет материала и выстави прозрачность.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/VisualExplosionMaterial.png" width="400"/>

3) Добавь в префаб еще один объект GrenadeModel. Это может быть что угодно, например модель из магазина или просто кубик. Главное, чтобы на этом объекте был коллайдер.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/GrenadeModel.png" width="600"/>

Создай скрипт [VacuumGrenadeLauncher.cs](https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/scripts/VacuumGrenadeLauncher.cs) и скопируй содержимое. Это такой же скрипт как и в прошлых вебинарах. При нажатии на правую кнопку мыши, скрипт создает копию префаба гранаты и поворачивает ее по линии прицела.

Навесь этот скрипт на объект Weapon в Player. Укажи ссылку на префаб гранаты

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/GrenadeLauncher.png" width="400"/>

Запусти сцену и проверь, что все работает
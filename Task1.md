# Задание 1: Гравитационная пушка!

## Описание

В этом задании мы реализуем механику гравитационной пушки. Будем притягивать любой объект с Rigidbody компонентом и выстреливать им с большой скоростью. Так же добавим мобам урон от столкновения с физическими объектами летящими с большой скоростью.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/task1.gif" width="600"/>

## Инструкция

1) Открой стартовую сцену. В этой сцене есть несколько врагов и работают базовые механики (кроме стрельбы)

Создай несколько объектов в сцене и добавь им компоненты Rigidbody. Это может быть что угодно, например обычные кубики

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/Cubes.png" width="600"/>

Выстави у этих объектов Collision Detection -> Continuous Speculative

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/Collision.png" width="400"/>

2) Создай скрипт [GravityGun.cs](https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/scripts/GravityGun.cs) и скопируй в него содержимое. Замени ??? на правильные фрагменты кода. Этот скрипт притягивает объект, в который мы стреляем лучом через прицел в центре экрана. Если мы еще раз нажимаем левую кнопку мыши, то мы отталкиваем предмет с большой скоростью.

Внутри объекта Player есть объект Weapon.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/WeaponGameObject.png" width="400"/>

Навесь GravityGun скрипт на объект Weapon.

<img src="https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/img/GravityGunComponent.png" width="400"/>

Теперь мы можем метать предметы во врагов. Но враги никак на это не реагируют! Модифицируй скрипт [EnemyHealth.cs](https://github.com/copetonrob/YP_Unity_M3_W11/blob/main/scripts/EnemyHealth.cs) так, чтобы при столкновении с объектом на высокой скорости враг получал урон.

4) Запусти сцену и проверь, что все работает.
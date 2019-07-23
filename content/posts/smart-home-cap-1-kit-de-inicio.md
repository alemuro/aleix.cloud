---
author: "Aleix Murtra"
date: 2019-07-21
title: Smart Home Cap. 1 - Kit de inicio
tags: ['domotica', 'iot']
draft: true
---

<!-- ![hola](../../img/capacitors-chip-circuit-board-57007.jpg) -->

Ha llegado el momento de empezar a automatizar cosas en casa. Tenemos la idea y estamos decididos: **queremos encender una bombilla al salir del trabajo**, creemos que eso puede resultar útil para informar a la gente que esté en casa de que estamos de camino. Además, creemos que es más fácil que automatizar la cafetera para que nos ~~despierte con el ruido~~ prepare un delicioso café a las 7 de la mañana.

Sobre el papel es muy fácil, únicamente necesitamos una bombilla, nuestra ubicación, automatizar el automatismo de alguna manera... Hay varias maneras de crear éste automatismo. Lo podemos hacer con un simple script/automatismo en [IFTTT](http://ifttt.com). Somos caprichosos y además vamos a querer disponer de un panel en el que ir añadiendo los _chismes_ que vayamos comprando, para tenerlo todo centralizado y poderlo controlar desde donde queramos. Podría ser que quisieramos pausar el automatismo o encender la bombilla en otro momento de manera manual.

## Bombilla 💡

Vale, queremos una bombilla, ¿pero cuál? Hay bombillas desde 10€ hasta de 50€ (y seguro que de más caras). ¿La queremos con Wifi, con Bluetooth o quizá con Zigbee? Las Zigbee suelen ser las bombillas más baratas, seguidas por las Bluetooth y finalmente las Wifi.

* Si es Wifi dependeremos de que el router no empiece a fallar, hay que vigilar con no llegar al límite de conexiones (sobretodo con 2.4G). Quizá deberemos crear una IP estática para cada dispositivo que queramos controlar si no queremos perder el control al reiniciar el router.
* Si es Bluetooth necesitamos que nuestro dispositivo de control tenga Bluetooth. La conexión se verá muy afectada por la distancia, no podremos poner dispositivos al otro lado de casa.
* Si es Zigbee nos veremos obligados a comprar un Hub, lo cual encarecerá la instalación sobretodo para controlar una única bombilla, nos obligará a comprar todos los dispotivios de la misma marca, si se estropea el hub nos quedaremos sin poder controlar todos los dispositivos asociados... 

## Raspberry Pi

Si, podemos usar otra placa que no sea Raspberry Pi, pero soy un fiel fan de éste tipo de chips.

* Raspberry Pi Zero W. Esta es la más barata. Está bien si no sabéis si vais a automatizar mucha cosa y para empezar. El principal problema es que tiene poca CPU y RAM, por lo que puede que se os quede corta rápidamente. A favor suyo, decir que tiene Wifi y Bluetooth por un precio muy bajo.

* Raspberry Pi 4 B. Aquí tendríamos la _joya de la corona_. La típica Raspberry con 1GB de RAM que casi puede con todo. ¿El principal problema? El precio.

* Raspberry Pi 3 A+. Éste es el model que yo me compré. Tiene una relación calidad/precio genial y no he llegado a su límite. En teoria no es tan potente como la B, pero hace su función sin ningún problema.
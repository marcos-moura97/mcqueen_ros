# Modelo do Relâmpago Marquinhos em URDF <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQdgBEX9U3kDSvXtCVyDqfA1uIlomS8rwJQCw&usqp=CAU" width="40" />

## Visão geral

O grande relâmpago marquinhos saiu das pistas da copa pistão diretamente para a sua simulação! Este modelo apresenta um simples conjunto de frames e o 
básico para que o robô possa andar. Caso queira adicionar algum sensor ao modelo, basta fazer isso no arquivo **relampago_marquinhos.urdf**.


## Requisitos

  - ROS Melodic
  - Catkin
  - Rviz
  - Gazebo
  
## Construir

Você deve seguir no terminal:

- Criar o espaço de trabalho catkin:

``` sh
$ mkdir catkin_ws
$ cd catkin_ws
$ mkdir src
$ catkin_make
```

- Clonar o repositório e a construí-lo:

``` sh
$ cd ~/catkin_ws/src
$ git clone https://github.com/marcos-moura97/mcqueen_ros.git
$ cd ..
$ catkin_make
```

## Visualizar no RVIZ

Para ver o modelo no RVIZ basta usar o comando


``` sh
$ roslaunch urdf_tutorial display.launch model:='$(find mcqueen)/urdf/relampago_marquinhos.urdf'
```

Será vista a imagem abaixo

![SLAM no ROS](/marquinhos.png "marquinhos")


## Lançar no Gazebo e mover com o teclado

O arquivo katiau.launch carrega o modelo no Gazebo, no RVIZ e também carrega o pacote **teleop_twist_keyboard** que dá a oportunidade de mover o modelo
usando algumas teclas. 

Para isso, devemos:

- Executar o roscore

``` sh
$ cd ~/catkin_ws/
$ source devel/setup.bash
$ roscore
```

- Lançar do programa

``` sh
$ roslaunch katiau.launch
```

## Mensagem final

<img src="https://media1.tenor.com/images/3af3a165800cb5a7a1c2bd2854729988/tenor.gif?itemid=5931942" width="200" />


# Lightning Mcqueen model in URDF <img src="https://www.championprofessional.com/wp-content/uploads/2015/07/en-icon.png" width="40" />

## Overview

The great Lightning McQueen, Relâmpago Marquinhos in portuguese, left the piston cup lanes directly for your simulation! This model features a simple 
set of frames and the basic so that the robot can walk. If you want to add a sensor to the model, just do it in the file **relampago_marquinhos.urdf**.

## Requirements

  - ROS Melodic
  - Catkin
  - Rviz
  - Gazebo

## To build

You must follow in terminal:

- Create the catkin workspace:

```sh
$ mkdir catkin_ws
$ cd catkin_ws
$ mkdir src
$ catkin_make
```

- Cloning the repository and building:

```sh
$ cd ~/catkin_ws/src
$ git clone https://github.com/marcos-moura97/mcqueen_ros.git
$ cd ..
$ catkin_make
```

## View on RVIZ

To see the model in RVIZ just use the command

``` sh
$ roslaunch urdf_tutorial display.launch model:='$(find mcqueen)/urdf/relampago_marquinhos.urdf'
```

The image below will be seen

![SLAM no ROS](/marquinhos.png "marquinhos")

## Launch in Gazebo and move with the keyboard

The katiau.launch file loads the model in Gazebo, RVIZ and also loads the **teleop_twist_keyboard** package which gives the opportunity to move the model
using a few keys.

For that, we must:

- Running roscore

```sh
$ cd ~/catkin_ws/
$ source devel/setup.bash
$ roscore
```

- Launching the program

```sh
$ roslaunch katiau.launch
```

## Final Message

<img src="https://media1.tenor.com/images/3af3a165800cb5a7a1c2bd2854729988/tenor.gif?itemid=5931942" width="200" />

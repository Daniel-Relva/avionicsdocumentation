---
id: arquitetura
title: Arquitetura
sidebar_label: Arquitetura
---

## Introdução
<br />
<br />
<br />

## Requisitos
<br />
<br />
<br />

## Nova REC
<br />
<br />
<br />

## Apogee Control System (ACS)
### ACS - Pitot Tube
<p>O tubo de Pitot fica na coifa do foguete e serve para calcular a <br>
velocidade de deslocamento, o que permite à aviônica se orientar e poder<br>
controlar de forma eficiente o airbreak.</p>

<p>Utilizando o príncipio de Bernoulli, podemos obter o valor da velocidade <br>
através de duas medidas distintas. Sendo elas a pressão estática e a pressão<br>
total. Ou seja, a pressão do fluido não sofrendo ação da velocidade do <br>
foguete e a pressão com ação da velocidade. </p>

<p>O modelo utilizado no Aurora Quimera é bem simples: dois sensores de <br>
pressão medindo cada tipo de pressão e um sensor de temperatura para <br>
controle de dados. Todos estes sensores são conectados à PMM, onde o Teensy <br>
irá calcular a velocidade e trabalhar em cima disso. </p>

<p>A temperatura será medida por um termopar tipo K e um  módulo Max6675.<br>
Até o momento, não foi possível determinar qual sensor de pressão será <br>
utilizado. Os principais candidatos são sensores de pressão absoluta ou <br>
transdutores de pressão.</p>

<p>A estimativa é que a pressão seja de aproxidamente 500KPa.</p>

#### Comunicação Coifa-Aviônica
<br />
<br />
<br />

### ACS - Air Brake
<br />
<br />
<br />

## Propulsion Sensing and Control System (PSCS)
<br />
<br />
<br />

### PSCS - Sensors
<p>O PSCS irá sensoriar tanto a pressão quanto a temperatura do tanque<br>
do oxidante e da câmara de combustão. Isso servirá para o microcontrolador<br>
Teensy possa controlar as válvulas de forma segura e eficiente.</p>

<p>O tanque terá uma temperatura de ambiente (até 40°) e uma pressão de 5 a<br>
5,8 MPa. Por estas razões, foi escolhido um transdutor PFT que mede até 10MPa<br>
e funciona até  100°C.</p>

<p>A câmara possui condições mais extremas. Com a combustão, temos uma <br>
temperatura de até 300°C e uma pressão que varia entre 3 MPa e 6 MPa. Por<br>
isso, foi utilizado um termopar tipo K com um Max6675 para medição de<br>
temperatura. Já a medição de pressão será feita com um sensor de pressão que<br>
funciona em altas temperaturas, que você pode encontrar com o nome de Type <br>
6025A.</p>

### PSCS - Valves
<br />
<br />
<br />

### PSCS - Ignition Sensing
<br />
<br />
<br />

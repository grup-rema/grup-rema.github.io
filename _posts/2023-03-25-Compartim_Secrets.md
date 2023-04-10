---
layout: post
title: Compartició de secrets per aprendre i portar a l’aula. - ReMA Pirineu
category: Sessions
tags:
  - competències
---
Presentació de Montse Alsina


Sessió 5 amb Montse Alsina. Compartició de secrets per aprendre i portar a l’aula.

**Compartició de secrets per aprendre i portar a l’aula.** 

*Taller impartit per Montse Alsina.*

En la societat actual tenim molt present que cal protegir dades i informació. En particular s'utilitzen mètodes per distribuir una informació secreta en un grup de participants de manera que cap d’ells té informació determinant del secret i es posen condicions sobre com han de cooperar entre ells per recuperar-lo. Ho anomenem compartició de secrets.

El que potser no tenim tan present, és quin paper hi juguen les matemàtiques i quina relació tenen amb les matemàtiques que treballem a les aules, especialment a secundària.

El repte de compartir secrets inclou tant la posada en comú (“compartir”) com el misteri i la complicitat que aporta el “secret”. Aquest problema es pot plantejar de moltes maneres i a molts nivells, des de primària com fins a la Universitat.

Volem generalitzar la manera de repartir un secret entre N persones, el qual es pot recuperar si es tenen m persones. Per tant, cal tenir en compte que necessitem :

- Que cada usuari tingui una part del secret
- Que el secret no doni més informació a un usuari i que sigui equitativa

Durant aquesta sessió, ens hem anat aproximant a solucions per a compartir secrets i alguns dels conceptes en els que podem aplicar el problema a l’aula.

1) APROXIMACIÓ VISUAL: No és una solució al problema però s’hi acosta.

Cada usuari té una part real de la imatge, encara que no complet. Si s’ajunten les imatges s’obté la informació final.

Exemple: Cada apartat pot ser blanc o negre, però no tothom tindrà el dibuix complet. Es poden donar els números de les caselles negres adjacents a cada fila i columna del dibuix (NONOGRAMS).



Una manera de no donar la informació real a cada un dels alumnes, seria tenir amb una part blanca i una part negra en el mateix. Amb dues imatges sobreposades s’aconseguiria el Secret.

Alguns dels conceptes treballats són:

- Mòdul 2 (sumes amb 0 i 1).
- Aritmètica

1) ESQUEMA DE SHAMIR

Es tracta de donar punts N usuaris per tal que ajuntant m usuaris, obtinguin el secret, S.


|<p>Per a m=2:</p><p>CONSTRUCCIÓ del SECRET</p><p>- triem 1 recta r: y=ax+S</p><p>- calculem punts de la recta</p><p>- donem un punt a cada usuari</p><p></p><p>RECUPERACIÓ del SECRET</p><p>- 2 usuaris posen els dos punts en comú</p><p>- calculen l’única recta que passa pels 2 punts r: y=ax+b</p>|
| :- |
|<p>Per a m=3:</p><p>CONSTRUCCIÓ</p><p>- triem 1 paràbola amb terme independent S</p><p>- calculem 1 punt de la paràbola per cada usuari</p><p>RECUPERACIÓ</p><p>- 3 usuaris posem els tres punts en comú</p><p>- utilitzen els sistemes d’equacions per a trobar a, b, c</p><p>- calculen l’única paràbola pels 3 punts.</p>|
|<p>Per a m qualsevol:</p><p>CONSTRUCCIÓ </p><p>- triem 1 polinomi de grau m-1 amb terme independent S</p><p>- calculem N punts i els repartim.</p><p>RECUPERACIÓ del secret</p><p>- m usuaris posen els m punts en comú</p><p>- calculem l’únic polinomi de grau m-1 pels m punts</p><p>- el secret és el terme independent</p><p></p>|

Alguns dels conceptes treballats són:

- Sistemes d’equacions
- Matrius i determinants
- Interpolació polinòmica
- Determinant de Vandermonde (nivell universitari)







1) ESQUEMA VECTORIAL DE BLACKLEY

El Secret serà un punt i caldrà amagar-lo entre un número infinit de punts.


|<p>Per a m=2:</p><p>CONSTRUCCIÓ del SECRET</p><p>- triem rectes del pla que passin pel punt S.</p><p>&emsp;- a cada usuari li donem una recta.</p><p></p><p>RECUPERACIÓ del SECRET</p><p>- punt de tall de les dues rectes</p>|
| :- |
|<p>Per a m=3:</p><p>CONSTRUCCIÓ</p><p>- triem plans que passin pel punt S.</p><p>&emsp;- a cada usuari li donem un pla	</p><p>RECUPERACIÓ</p><p>- 3 usuaris posem els tres plans en comú i busquen el punt d’intersecció.</p>|
|<p>Per a m qualsevol:</p><p>Es necessita donar espais de dimensions m-1 i serà necessari m-1 persones per a determinar el Secret.</p><p></p>|
|<p>Ampliació:</p><p>- Trobar quin pla és l’infiltrat (un d’ells és paral·lel)</p><p>- Que una persona tingui més plans que una altra (més facilitat per a trobar el secret)</p><p>- Donar plans que formin part d’un feix de plans a tothom i que només 1 persona tingui un pla diferent. Aquesta persona passaria a ser imprescindible per a determinar el punt.</p>|






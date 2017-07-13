# traceur-suspendu
Projet de traceur suspendu #Polargraph #DrawBot

## 1/ Kezako ?
<img src="https://dougkanter.files.wordpress.com/2011/11/vp1.jpg" alt="" style="width:100%" /><br />
<div style="text-align:right;color:#DDD;font-size:0.8em;">Crédit image : <a href="https://dougkanter.wordpress.com/2011/11/09/itp-icm-pcomp-final-project-concept/" target="_blank">Doug Kanter</a></div>

Le Polargraph (ou Traceur suspendu) est un robot qui dessine à votre place (un DrawBot).<br />
Il fonctionne à l'aide de 2 moteurs pas-à-pas reliés en triangulation avec un outil scripteur (un bloc-stylo quoi...) qui, en faisant évoluer la longueur des câbles qui les relient, permet de tracer sur une feuille.<br />
Le dispositif se tient verticalement et peut varier en dimensions : de la planche de travail à l'installation monumentale !

## 2/ État des lieux
J'ai commencé ce projet en juillet 2016 et après une phase de vortex, je l'ai laissé de côté... alors que le projet me passionne véritablement ^^<br />
J'ai en effet rencontré une série de problèmes techniques, que j'ai tenté de relever, en partie avec la communauté, mais je n'ai pas été capable de résoudre cet imbroglio seul :/

## 3/ Contribuez !
Si le projet vous intéresse et que vous souhaitez contribuer : contactez-moi ou retrouvons-nous @ La Fabrique du Loch !

## 4/ Comment ça (devrait) marche(r) ?

### # Impression 3D
Les éléments de montage à imprimer en 3D : axes, éléments de structure, tube pour le stylo...
### # Hardware
1 carte Arduino UNO + 1 shield pour les moteurs + 1 alimentation.
### # Firmware
1 Firmware adapté au shield, qui permettra le dialogue entre l'interface logicielle (sur ordi) et l'Arduino.
### # Interface logicielle
Elle traite les images et permet de les envoyer vers l'Arduino pour lancer le dessin. Elle permet également de paramétrer le traceur.

## 5/ Historique du projet
Dans un soucis pratique, j'ai décidé de partir sur un projet qui combine ces différents éléments. L'un ou l'autre des éléments m'importe peu : le tout est de les faire fonctionner ensemble... ce qui n'est pas le cas pour le moment :/<br />
Je me suis tout d'abord basé sur le travail de <a href="http://www.instructables.com/id/Polargraph-Drawing-Machine/" target="_blank">Euphy (Polargraph Drawing Machine)</a>.<br />
Voici ce que j'ai concrètement utilisé :

### # Impressions 3D


### # Hardware
État de fonctionnement : tout est OK.
* 1 Arduino UNO
* 1 <a href="https://cdn-learn.adafruit.com/downloads/pdf/adafruit-motor-shield-v2-for-arduino.pdf" target="_blank">Adafruit Motorshield v.2</a>
* 
### # Firmware

### # Interface logicielle

## 6/ Ou Ksa Kloch ?


## 7/ Références
* Le précurseur : <a href="http://juerglehni.com/works/hektor/" target="_blank">Hektor</a>, traceur-suspendu pour grapher (Street Art)
* <a href="https://tinkerlog.com/2011/09/02/der-kritzler/" target="_blank">Der Kritzler</a> [Tinkerlog] : un DrawBot sur une vitre
* <a href="http://www.polargraph.co.uk/" target="_blank">PolargraphSD</a>
* <a href="http://www.hackerspace-ffm.de/wiki/index.php?title=Drawbot@MfK" target="_blank">DrawBot@MFK</a>
* <a href="http://idlv.co/tipibot/" target="_blank">TipiBot</a> [Collectif IDLV / Rennes]
* Projet de <a href="http://makezine.com/2015/07/20/build-drawbot-two-cd-drives-raspberry-pi/" target="_blank">DrawBot avec 2 lecteur CD et 1 RaspberryPi</a>

## 8/ Contact
* Auteur : Guillaume | Twitter <a href="http://twitter.com/grouan" target="_blank">@grouan</a> | Mastodon <a href="http://mamot.fr/@grouan" target="_blank">@grouan</a><br />
* Lieu de fabrication : <a href="http://www.lafabriqueduloch.org" target="_blank">La Fabrique du Loch</a> (Auray)<br />
* Date : juillet 2016 (en stand by)


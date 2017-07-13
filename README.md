# traceur-suspendu
Projet de traceur suspendu #Polargraph #DrawBot by @grouan
<img src="https://raw.githubusercontent.com/grouan/traceur-suspendu/master/qrcode_projet_traceur_suspendu.png" alt="" style="float:right;" />

## 1/ Kezako ?
En vidéo ici https://www.youtube.com/embed/hQ8BQ0GsLiE ou ici https://www.youtube.com/watch?v=VufMgHvaoG0 ou encore là https://www.youtube.com/watch?v=2TiCZmJC9aU ...

Le Polargraph (ou Traceur suspendu) est un robot qui dessine à votre place (un DrawBot).<br />
Il fonctionne à l'aide de 2 moteurs pas-à-pas reliés en triangulation avec un outil scripteur (un bloc-stylo quoi...) qui, en faisant évoluer la longueur des câbles qui les relient, permet de tracer sur une feuille.<br />
Le dispositif se tient verticalement et peut varier en dimensions : de la planche de travail à l'installation monumentale !

## 2/ État des lieux
J'ai commencé ce projet en juillet 2016 et, après une phase de vortex (vous savez, cet espèce de vide sidéral...), j'ai du le laisser de côté... alors que suis totalement passionné par les robot dessinateurs (les DrawBots) de tous poils ^^<br />
J'ai en effet rencontré une série de problèmes techniques, que j'ai tenté de relever, en partie avec la communauté, mais je n'ai pas été capable de résoudre cet imbroglio dans sa globalité./<br />
<b>Je pense que le plus simple serait de repartir de zéro, de remettre à plat chaque étape pour avoir une vision globale cohérente et trouver les meilleurs solutions, plutôt que de tenter de mettre des rustines...</b>

## 3/ Contribuez !
Si le projet vous intéresse et que vous souhaitez contribuer : contactez-moi ou retrouvons-nous @ La Fabrique du Loch !
Scannez le QRCode ci-dessus si vous lisez ce document sur papier...

## 4/ Comment ça (devrait) marche(r) ?

### # Impression 3D
Les éléments de montage à imprimer en 3D : axes, éléments de structure, tube pour le stylo...
### # Hardware
1 carte Arduino UNO + 1 shield pour les moteurs (avec librairies pour Arduino) + 1 alimentation.
### # Firmware
1 Firmware adapté au shield, qui permettra le dialogue entre l'interface logicielle (sur ordi) et l'Arduino.
### # Interface logicielle
Elle traite les images et permet de les envoyer vers l'Arduino pour lancer le dessin. Elle permet également de paramétrer le traceur.

## 5/ Historique du projet
Dans un soucis pratique, j'ai décidé de partir sur un projet qui combine ces différents éléments. L'un ou l'autre des éléments m'importe peu : le tout est de les faire fonctionner ensemble... ce qui n'est pas le cas pour le moment :/<br />
Je me suis tout d'abord basé sur le travail de <a href="http://www.instructables.com/id/Polargraph-Drawing-Machine/" target="_blank">Euphy (Polargraph Drawing Machine)</a>.<br />
Voici ce que j'ai concrètement utilisé :

### # Impressions 3D
<img src="https://3dprint.com/wp-content/uploads/2015/05/ghizmo_drawbot_010_preview_featured.jpg" alt="" style="width:100%" /><br />
Les pièces que j'ai imprimées sont toutes tirées du projet de <a href="https://www.thingiverse.com/thing:798076" target="_blank">Polar DrawBot de DaGHIZmo</a> (sur Thingiverse). C'est ce qui me semblait être le plus complet, le plus documenté de A à Z, de l'impression à l'interface logicielle.

### # Hardware
État de fonctionnement : tout est OK.
* 1 Arduino UNO
* 1 <a href="https://cdn-learn.adafruit.com/downloads/pdf/adafruit-motor-shield-v2-for-arduino.pdf" target="_blank">Adafruit Motor Shield v.2</a> puis 1 autre Motor Shield usiné en Chine qui s'approche de la v.1 d'Adafruit (utilisé dans le projet que j'ai suivi et malheureusement plus en vente) + <a href="https://learn.adafruit.com/adafruit-motor-shield-v2-for-arduino/install-software" target="_blank">Adafruit Motor Shield Librabry</a>
* 2 <a href="https://www.adafruit.com/product/324" target="_blank">moteurs pas-à-pas NEMA-17</a> (Adafruit)
* 1 tout petit servo-moteur + 1 Futaba S3003 que j'ai de côté au cas où...
* quelques câbles, 2 chaînettes avec des billes plastiques (pour les engrenages)

### # Firmware
J'ai remixé le travail de <a href="https://twitter.com/aggrav8d" target="_blank">Dan ROYER</a> : <a href="http://www.makelangelo.com" target="_blank">Makelangelo</a>.<br />
Le <a href="https://github.com/MarginallyClever/Makelangelo-firmware" target="_blank">Firmware Makelangelo est téléchargeable</a> sur le Github de sont créateur.

### # Interface logicielle
Idem : j'ai récupéré le software de <a href="https://www.marginallyclever.com/product/makelangelo-software/" target="_blank">Makelangelo</a> (téléchargeable gratuitement en indiquant "CAD $0"). Bien sûr cela n'empêche par de soutenir ses projets en faisant une donation :)<br/>
J'ai essayé plusieurs versions, toutes fonctionnent sur l'ordi, semblent lancer une info au DrawBot, mais rien ne se passe...

## 6/ Références
* Le précurseur : <a href="http://juerglehni.com/works/hektor/" target="_blank">Hektor</a>, traceur-suspendu pour grapher (Street Art)
* <a href="https://tinkerlog.com/2011/09/02/der-kritzler/" target="_blank">Der Kritzler</a> [Tinkerlog] : un DrawBot sur une vitre
* <a href="http://www.polargraph.co.uk/" target="_blank">PolargraphSD</a> [Sandy Noble]
* <a href="http://www.hackerspace-ffm.de/wiki/index.php?title=Drawbot@MfK" target="_blank">DrawBot@MFK</a>
* <a href="http://idlv.co/tipibot/" target="_blank">TipiBot</a> [Collectif IDLV / Rennes]
* Projet de <a href="http://makezine.com/2015/07/20/build-drawbot-two-cd-drives-raspberry-pi/" target="_blank">DrawBot avec 2 lecteur CD et 1 RaspberryPi</a>
* Quelques photos des traceurs verticaux et horizontaux de <a href="https://www.flickr.com/photos/91789568@N00/" target="_blank">Kongorilla</a>

## 7/ Pour faire avancer le schmilblick
D'abord inspiré des travaux du Makelangelo, j'ai tendance à croire qu'il faut repartir du début. Heureux de constater que le projet du Collectif "Indiens Dans La Ville" (IDLV, artistes rennais) <a href="http://www.instructables.com/id/TIPIBOT-Le-Robot-Qui-Dessine/" target="_blank">le TipiBot, est désormais richement documenté sur Instructables</a>, je pense reprendre sur cette base !

<iframe src="https://player.vimeo.com/video/126355254" width="640" height="360" frameborder="0"></iframe>

* Impression 3D : à voir s'il est nécessaire que je réimprime... ?
* Hardware : Arduino UNO => MEGA 2560 ?
* Firmware : <a href="https://github.com/euphy/polargraph_server_polarshield" target="_blank">Polargraphe server polarshield</a> d'Euphy
* Software : <a href="https://github.com/RickMcConney/PenPlotter" target="_blank">PenPlotter</a> de Rick McConney


## 8/ Contact
* Auteur : Guillaume | Twitter <a href="http://twitter.com/grouan" target="_blank">@grouan</a> | Mastodon <a href="http://mamot.fr/@grouan" target="_blank">@grouan</a><br />
* Lieu de fabrication : <a href="http://www.lafabriqueduloch.org" target="_blank">La Fabrique du Loch</a> (Auray)<br />
* Date : 2016 (en stand by)
* <a href="https://www.lafabriqueduloch.org/forums/topic/traceur-suspendu-drawbot/" target="_blank">Post Forum La Fabrique du Loch</a>


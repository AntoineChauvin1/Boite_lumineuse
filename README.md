# Boite_lumineuse
Communication entre 2 esp8266 

Materiel

2 wemos d1 que nous nommerons W1 et W2

Le premier Wemos est constitué d’un interrupteur et d’une bande de led adressable.

Le second Wemos est constitué uniquement de 2 interrupteurs a et b



Principe de fonctionnement 

La bande de led adressable du W1 joue une séquence arc en ciel au repos.
L’appui sur le bouton de la W1 arrête la séquence et allume toute les leds en rouge.
Au relachement du bouton, la sequence arc en ciel reprend.
A chaque appui supplémentaire, toutes les leds passent ensuite au jaune, au vert, au bleu puis revient sur le rouge, etc…

Le deuxième wemos W2 doit se connecter en wifi au premier.
Lorsqu’il est Connecté, l’appui sur le bouton n’obéit plus au cycle Rouge, jaune vert bleu.
Il doit allumer la couleur en fonction des interrupteurs du W2

Interrupteur a : 0 interrupteur b : 0 couleur Rouge

Interrupteur a : 1 interrupteur b : 0 couleur jaune

Interrupteur a : 0 interrupteur b : 1 couleur vert

Interrupteur a : 1 interrupteur b : 1 couleur bleu

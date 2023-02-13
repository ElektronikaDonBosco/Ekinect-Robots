ATAZAK


1. HOME ASSISTANT

Lehenik eta behin, gure Raspberry Pi 4-an Home Assistant softwarea instalatu genuen.

1-Erantsi Home Assistant abiarazte-euskarria (SD txartela) ordenagailura

2-Deskargatu eta hasi Balena Etcher . (Agian administratzaile-pribilegioekin exekutatu beharko duzu Windows-en).

3-Hautatu "Flash URLtik" Hautatutako URLaren flasha erakusten duen Etcher softwarearen pantaila-argazkia.
![etcher1](https://user-images.githubusercontent.com/124257919/218414259-9466c2a2-4ba1-41b9-8b2c-67142bc3c6c4.png)


Lortu zure Raspberry Pi-ren URLa:

Raspberry Pi 4
Raspberry Pi 3
https://github.com/home-assistant/operating-system/releases/download/9.5/haos_rpi4-64-9.5.img.xz
Testua
Hautatu eta kopiatu URLa edo erabili gainean jartzen duzunean agertzen den "kopiatu" botoia.

Itsatsi zure Raspberry Pi-ren URLa Balena Etcher-en eta egin klik "Ados" Etcher softwarearen pantaila-argazkia URL barra itsatsita duen URLa erakusten duena.
Balena Etcherrek orain irudia deskargatuko du, hori amaitutakoan sakatu "Hautatu helburua" Etcher softwarearen pantaila-argazkia, hautatzeko xede-botoia nabarmenduta erakusten duena.
Hautatu zure Raspberry Pi-rako erabili nahi duzun SD txartela Etcher softwarearen pantaila-argazkia eskuragarri dauden helburuak erakusten dituena.
Egin klik "Flash!" irudia idazten hasteko Etcher softwarearen pantaila-argazkia Flash botoia nabarmenduta erakusten duena.
Balena Etcherrek irudia idazten amaitzean baieztapen hau jasoko duzu Etcher softwarearen pantaila-argazkia, instalazioa amaitu dela erakusten duena.
ABIARAZI ZURE RASPBERRY PI
Sartu sortu berri duzun abio-euskarria (SD txartela).

Lotu Ethernet kable bat sarerako.

Lotu elikadura-kablea.

Zure Mahaigaineko sistemako arakatzailean, minutu gutxiren buruan zure Etxeko Laguntzailea eginbide berriari heldu ahal izango diozu homeassistant.local:8123 helbidean .

Windows bertsio zaharrago bat exekutatzen ari bazara edo sarearen konfigurazio zorrotzagoa baduzu, baliteke Home Assistant-era atzitu behar izatea homeassistant:8123 edo http://X.X.X.X:8123(ordezkatu XXXX zure Raspberry Pi-ren IP helbidearekin).
Home Assistant Sistema Eragilea instalatuta eta eskuragarri dagoenez, sartzearekin jarraitu dezakezu.


ATAZAK


1. HOME ASSISTANT

Lehenik eta behin, gure Raspberry Pi 4-an Home Assistant softwarea instalatu genuen.

1-Erantsi Home Assistant abiarazte-euskarria (SD txartela) ordenagailura

2-Deskargatu eta hasi Balena Etcher . (Agian administratzaile-pribilegioekin exekutatu beharko duzu Windows-en).

3-Hautatu "Flash URLtik" Hautatutako URLaren flasha erakusten duen Etcher softwarearen pantaila-argazkia.
![etcher1](https://user-images.githubusercontent.com/124257919/218414259-9466c2a2-4ba1-41b9-8b2c-67142bc3c6c4.png)

4-Lortu zure Raspberry Pi-ren URLa:

![image](https://user-images.githubusercontent.com/124257919/218414503-86ea5052-64ea-4cbb-ada7-20dd810176d2.png)


Hautatu eta kopiatu URLa edo erabili gainean jartzen duzunean agertzen den "kopiatu" botoia.

1.Itsatsi zure Raspberry Pi-ren URLa Balena Etcher-en eta egin klik "Ados" 
![etcher2](https://user-images.githubusercontent.com/124257919/218414702-50a26829-4a2e-4264-8093-a836be9b2796.png)

2.Balena Etcherrek orain irudia deskargatuko du, hori amaitutakoan sakatu "Hautatu helburua"
![etcher3](https://user-images.githubusercontent.com/124257919/218414933-4d497066-f63d-4326-ba53-dfd714c748ee.png)

3.Hautatu zure Raspberry Pi-rako erabili nahi duzun SD txartela
![etcher4](https://user-images.githubusercontent.com/124257919/218415116-bfe89a2f-9a96-4fef-b96d-7f5932fdbd92.png)

4.Egin klik "Flash!" irudia idazten hasteko
![etcher5](https://user-images.githubusercontent.com/124257919/218415248-f965962d-9646-4c80-bb79-656b86fd7954.png)

5.Balena Etcherrek irudia idazten amaitzean baieztapen hau jasoko duzu Etcher softwarearen pantaila-argazkia, instalazioa amaitu dela erakusten duena.
![etcher6](https://user-images.githubusercontent.com/124257919/218415564-b5b52126-0598-4cb2-800a-4a5ee4e13c69.png)

ABIARAZI ZURE RASPBERRY PI

1.Sartu sortu berri duzun abio-euskarria (SD txartela).

2.Lotu Ethernet kable bat sarerako.

3.Lotu elikadura-kablea.

4-Zure Mahaigaineko sistemako arakatzailean, minutu gutxiren buruan zure Etxeko Laguntzailea eginbide berriari heldu ahal izango diozu homeassistant.local:8123 helbidean.
- Windows bertsio zaharrago bat exekutatzen ari bazara edo sarearen konfigurazio zorrotzagoa baduzu, baliteke Home Assistant-era atzitu behar izatea homeassistant:8123 edo http://X.X.X.X:8123(ordezkatu XXXX zure Raspberry Pi-ren IP helbidearekin).
Home Assistant Sistema Eragilea instalatuta eta eskuragarri dagoenez, sartzearekin jarraitu dezakezu.


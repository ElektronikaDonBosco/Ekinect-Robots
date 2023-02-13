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

5.Balena Etcherrek irudia idazten amaitzean baieztapen hau jasoko duzu Etcher softwarearen pantaila-argazkia, instalazioa amaitu da
![etcher6](https://user-images.githubusercontent.com/124257919/218415564-b5b52126-0598-4cb2-800a-4a5ee4e13c69.png)

ABIARAZI ZURE RASPBERRY PI

1.Sartu sortu berri duzun abio-euskarria (SD txartela).

2.Lotu Ethernet kable bat sarerako.

3.Lotu elikadura-kablea.

4-Zure Mahaigaineko sistemako arakatzailean, minutu gutxiren buruan zure Etxeko Laguntzailea eginbide berriari heldu ahal izango diozu homeassistant.local:8123 helbidean.
- Windows bertsio zaharrago bat exekutatzen ari bazara edo sarearen konfigurazio zorrotzagoa baduzu, baliteke Home Assistant-era atzitu behar izatea homeassistant:8123 edo http://X.X.X.X:8123(ordezkatu XXXX zure Raspberry Pi-ren IP helbidearekin).
Home Assistant Sistema Eragilea instalatuta eta eskuragarri dagoenez, sartzearekin jarraitu dezakezu.

1.1 ZIGBEE

![logo](https://user-images.githubusercontent.com/124257919/218418768-e6cd0f7e-137a-4f9b-b579-0325b77207f6.png)

1- Oraindik ez baduzu MQTT artekaririk; Home Assistant-en joan Ezarpenak → Gehigarriak → Gehigarrien denda eta instalatu Mosquitto broker gehigarria.

2- Itzuli Gehigarrien dendara , egin klik ⋮ → Biltegiak , bete https://github.com/zigbee2mqtt/hassio-zigbee2mqtteta egin klik Gehitu → Itxi .

3- Biltegiak bi gehigarri ditu:
  · Zigbee2MQTT Zigbee2MQTT kaleratutako bertsioen jarraipena egiten duen bertsio egonkorra da. ( erabiltzaile gehienentzat gomendatua )
  · Zigbee2MQTT Edge -k Zigbee2MQTT- ren devadarraren jarraipena egiten du, ertz-bertsioa instalatu dezakezu oraindik kaleratu ez diren Zigbee2MQTT dev adarrean eginbide edo konponketak badaude.
  
4- Egin klik gehigarrian eta sakatu Instalatu eta itxaron gehigarria instalatu arte.

5- Egin klik Konfigurazioan:
  · Mosquitto broker gehigarria erabiltzen ez baduzu , bete zure MQTT xehetasunak (utzi hutsik Mosquitto broker gehigarria erabiltzean). Formatua hemen aurki daiteke , baina saltatu hasierako mqtt:koska. adibidez:

      server: mqtt://localhost:1883
      user: my_user
      password: my_password
      
  · Bete serieko xehetasunak (adibidez, zure USB koordinatzailearen ataka). Formatua hemen aurki daiteke , baina saltatu hasierako serial:koska. adibidez:

      port: /dev/ttyUSB0

  · Portua ezagutzen ez baduzu eta USB gailu bakarra baduzu zure makinara konektatuta, saiatu /dev/ttyUSB0. Bestela, erabili Home Assistant CLI eta exekutatu ha hardware infojakiteko.

  · Sakatu Gorde

  · Aholkua: Home Assistant fitxategiko aldagaiak aipatzea posible da secrets.yaml(ez Zigbee2MQTT!) erabiliz, adibidez.password: '!secret mqtt_pass'

6- Hasi gehigarria Informaziora joan eta sakatu Hasi

7- Itxaron Zigbee2MQTT abiarazi arte eta sakatu IREKI WEB UI Zigbee2MQTT behar bezala hasi dela egiaztatzeko.

  · Erakusten badu, 502: Bad Gatewayitxaron pixka bat gehiago eta freskatu orria.
  
  · Honek luzeegia hartzen badu (adibidez, 2 minutu +), egiaztatu Erregistroa fitxan zer gertatu den gaizki ikusteko.
  
 1.2 ESP HOME
 
 Gure sentsoreen sarea egiteko "Esp Home" aplikazioa instalatu genuen.
 
 1- "Osagarri-denda" sartu eta bilatzailean EspHome jarri
 
 ![image](https://user-images.githubusercontent.com/124257919/218420948-516ea4e7-5a26-44d1-b910-adb6acd908d7.png)
 
 2- EspHome instalatu eta hasi
 
 ![image](https://user-images.githubusercontent.com/124257919/218422064-ddfe6e61-61ee-4c15-86f8-3bdeb50fd9f8.png)

 3- EspHome barruan, gailuak jartzeko. "Gailua gehitu" botoiari eman eta daukazuten plaka mota aukeratu.
 
 ![image](https://user-images.githubusercontent.com/124257919/218422678-01527f06-0b3e-4241-945d-cec5958dabab.png)
 
 4- Yaml programa jartzeko, interneteko bilatzailean "esphome" bilatu eta aterako den web-gunean zure sentsorea bilatu.
 
 ![image](https://user-images.githubusercontent.com/124257919/218423518-d918e61e-31d7-4889-8ca3-1366b8785506.png)
 
 1.3 Node-Red
 
 1- Node-Red instalatzeko; Home Assistant-en joan Ezarpenak → Gehigarriak → Gehigarrien denda eta instalatu Node-Red.

 2- Node-Red konfiguratzeko:

· credential_secret*-en pasahitz bat idatzi behar duzu, hainbat elementu kodetzeko erabiliko dena.
![image](https://user-images.githubusercontent.com/124257919/218424770-6081787e-b7f0-493c-8fd9-dfcdb281d9d3.png)

· http_node:
	password: zuen Home Assitanteko pasaitza
	username: zuen Home Assistanteko erabiltzaile izena
![image](https://user-images.githubusercontent.com/124257919/218424849-19881dfa-a7f7-4a76-a7c0-57b72285dd60.png)

· http_static:
	password: zuen Home Assitanteko pasaitza
	username: zuen Home Assistanteko erabiltzaile izena
![image](https://user-images.githubusercontent.com/124257919/218424956-82b741e4-63f2-4040-874a-11113dca680a.png)

  3- Red konfigurazioan portua 1880 jarri behar da.
![image](https://user-images.githubusercontent.com/124257919/218424595-3e511ec3-90fe-465c-a0c7-7b0b17321736.png)


2. PROTEUS

Barruko plakaren konexioak

![1_k_JmJsVBnjiRLG1Snjm8vQ](https://user-images.githubusercontent.com/124257919/218435704-e342d077-ba37-4c9c-91d3-df3c3d1533a3.png)



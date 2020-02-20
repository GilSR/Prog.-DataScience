# Prog.-DataScience
Repositori amb docker file imitant VM assignatura UOC Programacio per a la ciencia de dades

S'ha intentat mantenir les mateixes versions que a la VM pero en alguns casos no ha estat possibe.
Aixi mateix, la imatge no inclou els arxius de la carpeta "geoplotlib_tiles/positron". Pot mirar de ser inclos mes endavant.


## Posada en marxa

1. Instal·lar [docker](https://docs.docker.com/install/)
2. Obrir un terminal a la carpeta on es vulgui desar els arxius del curs.
3. Executar des del terminal: *git clone https://github.com/sineline/Prog.-DataScience.git Prog_DS*
4. Introduir la comanda *cd Prog_DS*
2. Executar la comanda *docker-compose up -d* (sense -d per debug)

# Utilitzacio

Un cop executada la maquina, es pot accedir a aquesta a traves de http://localhost:8888/
En cas de problemes accedint a localhost, [mirar aquest enllaç](https://stackoverflow.com/questions/7580508/getting-chrome-to-accept-self-signed-localhost-certificate)

Un cop creada la maquina, els notebooks seran desats per defecte a la carpeta /PEC/ de la ruta on es troba l'arxiu docker-compose.yml, des d'on s'ha executat la comanda d'arrancada.

## Descarrega de noves PECs (Un cop el contenidor ja ha estat creat)
#### Opcio 1:
1. Obre el terminal a la ubicacio dels arxius descarregats.
2. Executa la comanda *docker-compose run UOC_AdvPython get_pec.sh*

#### Opcio 2:
1. Obre un nou terminal des de jupyter-notebook (New > Terminal)
2. Executa la comanda *get_pec.sh*

## Instal·lacio de nous paquets per python
1. Obre el terminal
2. Executa *docker-compose run UOC_AdvPython python3 -m pip install **nom del paquet***

## Accedir a la maquina per consola
1. Obre el terminal a la ubicacio dels arxius del curs.
2. Executa la comanda *docker-compose run UOC_AdvPython sh*

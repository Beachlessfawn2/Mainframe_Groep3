# DB2 info sessie:

## spufi

* Dataset name -> eerst zelf nuttig dataset maken. (member hoeft nog niet). VB: 'HOG0033.SPUFI.INPUT1'
* Output data set name -> GEEN PDS. WSS undifiened. Moet nog aangemaakt worden(volledig/ ook member).
* Options: (yes/no geeft aan al dan niet uitvoeren. * -> betekend dat het reeds uitgevoerd is.)
	1. change defauls -> een aantal opties over het proces
	2. edit input -> om input te gaan aanpassen zoals ispf editor.
	3. execute -> uitvoeren van proces.
	4. autocommit -> automatisch toepassen.
	5. browse output -> Kunt ge gaan kijken naar de output van het proces.

## Spufi.output

org: ps
refm: VB
recl: 4092
BS: 4096
first extent: 1
Second tracks: 5
DirBlck: 10

## Maken DB Querry

* STOGROUP -> UNIHOGSG
* Unieke naam keizen voor de database!!!
* FK -> alter table NAME
	edd constraint fk_NAME
	foreign key (soort_id)
	references soort38;
* PK -> primary key ()
	in database NAME;

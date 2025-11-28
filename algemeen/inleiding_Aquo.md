# De Aquo-standaard

De Aquo-standaard (Aquo) is de Nederlandse standaard voor het uitwisselen van gegevens binnen de watersector.  
Informatie is een belangrijke motor voor het functioneren van de watersector. Steeds meer en verschillende overheidslagen en instanties werken samen en wisselen informatie uit. Daarom is het belangrijk dat we allemaal dezelfde betekenis geven aan de gegevens en woorden die we gebruiken. En dat we gemeenschappelijke afspraken maken over hoe we gegevens beschrijven en de manier waarop we ze uitwisselen.

Dankzij de Aquo-standaard is het mogelijk om op een uniforme en efficiënte manier gegevens uit te wisselen tussen partijen die betrokken zijn bij waterbeheer. Bovendien maakt toepassing van de standaard het mogelijk om informatie zo te ordenen en te beheren dat de actualiteit, juistheid en consistentie van die informatie wordt geborgd.  
De Aquo-standaard draagt daarmee bij aan de kwaliteit van het waterbeheer. Het eenvoudig en eenduidig delen van informatie levert voordeel op in tijd en geld.

Aquo is voor overheidsorganisaties een verplichte open standaard, die is ontwikkeld en wordt beheerd door het Informatiehuis Water. Het Informatiehuis Water is een samenwerkingsprogramma van Rijkswaterstaat, de waterschappen en de provincies.  
Het Informatiehuis Water ontzorgt waterbeheerders en beleidsmakers bij het uitwisselen van waterinformatie.

## Het Informatiemodel Water (IMWA)

Het Informatiemodel Water (IMWA) vormt de basis van de Aquo-standaard. IMWA is voornamelijk een informatiemodel voor geo-informatie en is dan ook gebasseerd op de NEN3610:2022 Basismodel geo-informatie. IMWA biedt de basis voor de informatiestructuur die binnen de gegevensuitwisseling wordt gebruikt. Om dit te kunnen doen beschrijft IMWA de concepten waarover informatie uitgewisseld moet worden binnen het waterbeheer, onderlinge relaties tussen deze concepten en eigenschappen over deze concepten.

IMWA is een omvangrijk informatiemodel. Om overzicht te houden wordt het onderverdeeld in 3 taakgebieden:
- [IMWA Watersysteem](https://aquo-standaard.github.io/IMWA-WS/#inleiding)
- IMWA Waterketen (nog te ontwikkelen)
- IMWA Waterveiligheid

Daarnaast zijn of worden een aantal onderdelen gemodelleerd ter ondersteuning van die taakgebieden:
- [IMWA Kunstwerken](https://aquo-standaard.github.io/IMWA-KW/)
- [Nederlands profiel Observaties, Metingen en Monsters voor de watersector](https://aquo-standaard.github.io/OMM-W/)
- IMWA Normen
- IMWA Maatregelen

Elk onderdeel heeft een connectie met het IMWA Basis.  IMWA Basis vormt de fundering van het IMWA. In onderstaande afbeelding zie je de samenhang tussen de verschillende onderdelen. [Catalogus IMWA Basis](https://aquo-standaard.github.io/IMWA-basis/#cat)
**Let op!** Dit is nog niet de definitieve versie van IMWA. De doorontwikkeling van het IMWA kan nog tot veranderingen leiden.

In de onderstaande afbeelding is een (voorlopige) weergave te zien van IMWA en de samenhang tussen de verschillende onderdelen binnen IMWA. Let op! Dit is nog niet de definitieve versie van IMWA en is onderheven aan veranderingen die tot stand komen door de verdere doorontwikkeling van IMWA.

![De context van IMWA](./algemeen/Aquomodellenoverzicht.jpg)
*Totaalplaat van IMWA in samenhang*

## MIM-conform

De Aquo-informatiemodellen zijn opgezet volgens het **MIM - Metamodel Informatie Modellering** ([geostandaarden.nl](https://docs.geostandaarden.nl/mim/mim/)). MIM biedt een gemeenschappelijk vertrekpunt voor het maken van informatiemodellen. De afspraken reiken over de grenzen van bestuurslagen heen en zijn toepasbaar in uiteenlopende domeinen. Het volgen van MIM zorgt er ook voor dat er een gelaagdheid is aangebracht in de informatiemodellen

- **Conceptueel model**: Hierin wordt de informatie beschreven die van belang is binnen een bepaald werkveld. Het definieert het 'wat': welke concepten worden onderscheiden in een bepaald werkveld, wat betekenen deze, hoe verhouden deze zich tot elkaar en welke informatie over deze concepten belangrijk is. 
- **Logisch model**: Dit is een afleiding van het conceptuele model, die is gemaakt voor een specifieke toepassing. Het defineert het 'hoe': binnen een logisch model wordt beschreven hoe de concepten die binnen het conceptueel model gedefineerd zijn, worden gebruikt binnen systemen en tussen systemen, bijvoorbeeld voor databases en in de uitwisseling daartussen. Het logisch model beschrijft niet de technische implementatie van het model in systemen, maar is een eerst aanzet daartoe.
- **Fysiek model**: Hierin worden de structuur en eigenschappen van een daadwerkelijk technologie beschreven waarin de informatie wordt vastgelegd of uitgewisseld. Hte bschrijft bijvoorbeelde sturctuur van een database of uitwisselbericht.

Zie voor verdere toelichting:  
[Metamodel Informatie Modellering](https://docs.geostandaarden.nl/mim/mim/)

De Aquo-informatiemodellen zijn gemodelleerd met behulp van **UML (Unified Modeling Language)** in **Enterprise Architect**.

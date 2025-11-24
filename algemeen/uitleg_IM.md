# Modelelementen

Modelelementen zijn de bouwstenen van een informatiemodel. Ze bepalen de structuur en werking van het model. Elk element heeft een specifieke functie binnen het informatiemodel en daarmee ook in het beheer van data.  

Elk informatiemodel heeft een aantal vaste elementen. Door deze elementen goed te begrijpen, wordt het model en de catalogus makkelijker te lezen.

## Objecttypen

Een object is een modelelement dat wordt gebruikt om de objecten waarover wordt gesproken in een specifiek werkveld te modelleren (voor de watersector bijvoorbeeld een oever, een waterbodem, een observatie, een norm etc.). Deze objecttype hebben bijna altijd eigenschappen die wij attributen noemen. D Deze objecttypen hebben altijd relaties met elkaar. Deze relaties zorgen er voor de alle objecten in het model in samenhang worden gebracht en een betekenisvolle eenheid vormen. In het model zijn dit de verschillende blokken die zijn aangeduid als *Objecttype*.

##Attribuut

Een attribuut is een eigenschap of kenmerk van een object. Deze eigenschappen weergeven de informatie die een waterbeheerder wil uitwisselen over een bepaald object (bijvoorbeeld de breedte van een kunstwerk, het type wandconstructie). In het model worden deze eigenschappen weergeven in de objecttype met de aanduiding *Attribuutsoort*.

##Datatypen

Een datatype is altijd verbonden aan een attribuut. Het datatype bepaald in wat voor vorm/in wat voor waarde een attribuut uitgewisseld kan worden. Enkele datatypen die voorkomen in IMWA zijn:

- `integer` (geheel getal)
- `characterstring` (tekst)
- `date` (datum)
- `year` (jaar)
- `GM_Object` (geometrie)
- `measure` (waarde & eenheid)
- `type....` (Aquo-domeintabel)

Er wordt een verschil gemaakt tussen *primitieve datatypen* complexe datatypen. Primitieve datatypen zijn eenvoudige datatypen die bestaan uit één element zoals een integer bestaat uit enkel één getal. Complexe datatypen bestaan uit twee of meer elementen bijvoorbeeld, een measure bestaat uit een getal en een eenheid. In het model worden deze datatypen weergeven bij de attributen met de aanduiding *Datatype*.

Naast deze datatypen kunnen attributen gekoppeld zijn aan een Aquo-domeintabel. Bij een attribuut moet dan een waarde uit de aangegeven Aquo-domeintabel worden aangegeven bijvoorbeeld, attribuut typeSluis verwijst naar de domeintabel SluisType waaruit de waarde keersluis kan worden gekozen.

##Gegevensgroepen
Soms worden meerdere attributen gegroepeerd in een *gegevensgroep*. De attributen in zo’n groep horen inhoudelijk bij elkaar en worden als een geheel behandeld bijvoorbeeld, de gegevensgroep *afmetingen*, waarin de attributen *lengte*, *breedte* en *hoogte* zitten. Gegevensgroepen kunnen bij meerdere objecttypen tegelijk  worden gebruikt.

## Relaties

Objecten kunnen aan elkaar gekoppeld zijn via relaties. Een relatie heeft altijd een richting. In de meeste gevallen loopt deze van een *bron* naar een *doel*.  

De meest voorkomende relatie in IMWA is de *generalisatie*. Soms komt ook een *associatierelatie* voor.

![Generalisatie en Associatie](algemeen/GeneralisatieAssociatie.jpg)
*Voorbeeld van generalisatie- en associatierelatie.*

- **Generalisatierelatie**  
  Een generalisatierelatie geeft aan dat een object afgeleid is van een ander object. Dit betekent dat de eigenschappen van het ene object ook gelden voor het andere object. Dit wordt een *'is-een'-relatie* genoemd.  

- **Overerving**  
  Overerving betekent dat een object eigenschappen erft van een ander object. In het voorbeeld erft *WaterstaatkundigeZonering* alle eigenschappen van *IMWA-GeoObject*. Het verschil is dat *WaterstaatkundigeZonering* extra eigenschappen heeft.

- **Abstract object**  
  Een abstract object is een object dat niet als zelfstandig element voorkomt in de echte wereld. Het wordt gebruikt als sjabloon voor andere objecten. In het model krijgen abstracte objecten vaak een samengestelde naam die cursief wordt weergegeven.

- **Associatierelatie**  
  Een associatierelatie beschrijft een *heeft-een*-relatie tussen twee objecten. Deze relatie geeft aan dat de objecten samenwerken, maar niet per se een hiërarchische relatie hebben.  
  In associatierelaties speelt *kardinaliteit* een rol. Kardinaliteit geeft aan hoeveel objecten met elkaar verbonden zijn. Dit wordt weergegeven in de notatie `n..m`. Als er geen kardinaliteit staat, wordt aangenomen dat deze `1..1` is.

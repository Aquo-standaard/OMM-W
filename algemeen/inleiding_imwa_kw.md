# Informatiemodel Water (IMWA) Kunstwerken

Een van de domeinen of werkvelden in het informatiemodel water (IMWA) is het onderdeel Kunstwerken.

Zie voor verdere toelichting van de samenhang tussen de verschillende domeinen in de IMWA bij IMWA Basis:  
[Catalogus IMWA Basis](https://aquo-standaard.github.io/IMWA-basis/#cat)

IMWA Kunstwerken beschrijft de fysieke objecten in de werkelijkheid en de bijbehorende fysieke eigenschappen. Oftewel, de werkelijke kunstwerken die zichtbaar en tastbaar zijn in het landschap met hun uiterlijke kenmerken zoals bijvoorbeeld het type en de afmeting.

Uiteraard is er meer relevante informatie om vast te leggen over een kunstwerk, bijvoorbeeld welke functie(s) het object heeft, wie de beheerder is of wat de toestandsbeoordeling is van het object. Dit zijn echter geen fysieke eigenschappen en daarom niet opgenomen in dit onderdeel van IMWA. Dit type informatie is vastgelegd in de andere onderdelen van IMWA zoals ‘Basis’, ‘Watersysteem’, ‘Waterveiligheid’ of ‘Monitoring’. Het onderdeel Kunstwerken is dan ook nauw verbonden met de andere onderdelen van IMWA.

Door deze nauwe relatie kan er wel iets worden gezegd over een kunstwerk binnen een bepaalde context, zoals de rol en functie, zonder dat dit dubbel gemodelleerd is. Een voorbeeld hiervan is dat een sluis niet alleen een kunstwerk is, maar ook een waterkerende functie heeft binnen de context van waterveiligheid.

Kunstwerken heeft ook betrekking op de elementen waaruit een kunstwerk kan bestaan. Hierdoor richt Kunstwerken zich dus ook op de decompositie van kunstwerken. Er is voor gekozen om de decomposities van de kunstwerken te beperken tot onderdelen die van belang zijn voor de werking en beoordeling van een kunstwerk vanuit het perspectief van waterbeheer. Een verdere decompositie, zoals bijvoorbeeld schroeven en scharnieren, wordt binnen andere standaarden zoals de NEN2767-4 vastgelegd.

# Modelleerbeslissingen en openstaande acties

## Modelleerbeslissingen

1. **IMWA bevat een eigen object Kunstwerk** dat een specialisatie is van het NEN3610:2022 object Kunstwerk. Dit hoort zo gemodelleerd te worden. De specialisatie IMWA object Kunstwerk deelt daarmee alle eigenschappen met het NEN3610:2022 object Kunstwerk, zoals attributen en de definitie.
2. **IMWA Kunstwerken bevat een beperkte decompositie** die voldoende is voor de huidige uitwisseldoelen in het waterbeheer. Voor het vastleggen van asset informatie bestaan andere standaarden zoals de NEN2767-4 en IEC/ISO 81346 - Reference Designation System (RDS). De Aquo-standaard sluit hier nog niet op aan, omdat er op dit moment geen uitwisseldoel is voor deze informatie. Mocht dit in de toekomst nodig zijn dan kan dit worden aangevraagd bij de servicedesk van het Informatiehuis Water.
3. **Op verzoek van gebruikers is een relatie gelegd tussen IMWA en BGT|IMGeo**. Het gaat om:
   - Kunstwerk (IMWA) en functioneel gebied (BGT|IMGEO)
   - Kunstwerk element (IMWA) en Kunstwerkdeel (IMWA en BGT|IMGEO)

## Openstaande acties
Tijdens de publieke consultatie zijn een aantal vragen gesteld waarvoor meer informatie nodig is om deze uit te kunnen werken in het informatiemodel. Deze gebruikersvragen staan hieronder. We willen deze in samenwerking met de waterbeheerders gaan uitwerken voor de volgende versie van IMWA Kunstwerken.

Heb je een idee over of een antwoord op één van deze gebruikersvragen, of wil je uitgenodigd worden om mee te praten? Stuur dan een bericht met je feedback of aanmelding naar [servicedesk@ihw.nl](mailto:servicedesk@ihw.nl).

1. Er ontbreken nog attributen bij duiker. Welke zijn dit?
2. De wens is om aan te kunnen geven om wat voor opening het gaat bij het object Doorstroomopening. Op welke manier moet dit worden aangegeven?  
   - Een attribuut `typeOpening` met een domeintabel (bijv. Hoofdopening en Nevenopening).  
   - Of een attribuut `hoofdopening` met een ja/nee optie.
3. De wens is om bij Duiker, Sifon of Hevel het constructiemateriaal uit te kunnen wisselen. Welke materialen moeten hiervoor worden opgenomen in een domeintabel? Zijn er nog meer materialen nodig?
4. Moet er een object Steiger worden opgenomen? Welke eigenschappen moeten dan kunnen worden uitgewisseld (bijv. materiaal, type, afmeting)?
5. Welke attributen ontbreken bij het object Overgangsconstructie?
6. Is er behoefte om de volgende objecten toe te voegen aan het model, onder Kunstwerk-element? Welk uitwisseldoel hoort hierbij?  
   - Grof Zand Barrière (GZB)  
   - Verticaal Zanddicht Geotextiel  
   - Filterconstructies/grindkoffers  
   - Ontlaststelsels (anders dan drainagebuizen)  
   - Kleiingravingen/grondverbeteringen (kleikisten, kleiingravingen, etc.)  
   - Dijkvernageling  
   - Langsconstructies  
   - Palenwanden  
   - Anti-graverij voorzieningen (bevergaas etc.)  
   - Funderingsconstructies (bijv. fundering onder een L-wand of gemaal)
7. Hoe kan worden aangegeven op welke manier een afsluitmiddel een doorstroomopening beïnvloedt?  
   - Een optie is het toevoegen van attributen zoals `ingeregeldeHoogte`, `ingesteldeHoogte`, `ingesteldeBreedte`, `hoogteDrempelAfsluitmiddel`.
8. Gaat erosieBestendigheid over een materiaal of een beoordeling van de staat van de afdeklaag? Voor welk doel moet dit worden uitgewisseld?
9. Een bekkentrap, een type vispassage, heeft ook een waterregulerende functie. Moet dit worden opgenomen?
10. Wat is het uitwisseldoel van het object (Rooster)reinigingsinstallatie? Moet dit worden toegevoegd?
11. Brug blijkt niet eenduidig opgenomen in het model. Er zijn drie aspecten:
    - **Het type overspanning van een brug** (is opgenomen in model).
    - **Het daadwerkelijke type brug** (is opgenomen, maar loopt door elkaar met de techniek die wordt gebruikt om een brug te openen/sluiten).
    - **De techniek van openen/sluiten** (niet expliciet opgenomen).
12. Hoe kunnen leidingkruisingen toegevoegd worden aan het model in relatie tot dijken? Moet IMWA aansluiten op IMKL (Informatiemodel Kabels en Leidingen)?
13. Welke domeinwaarden horen er bij de objecten?  
    - AansluitconstructieType  
    - AfdeklaagMateriaalType  
    - GeotextielMateriaalType  
    - KokervormType  
    - PompType  
    - VlijlaagUitvullaagMateriaalType  
    - ToplaagMateriaalType  
    - KernOpbouwType  
14. De domeinwaarden hebben nog geen definitie. Wie wil deze reviewen nadat ze zijn opgesteld?
15. Wij zoeken gebruikers die mee willen denken over het modelleren van gemalen. De types gemalen, pompen en bemalingen hebben overlap, wat voor verwarring zorgt.

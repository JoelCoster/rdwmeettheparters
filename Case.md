_Dutch, English below_

---

# Mastje branden

## Achtergrond
Zoals vele andere (semi-)overheden, heeft de RDW een grote hoeveelheid [open data](https://opendata.rdw.nl/) online staan. Hierbij kan je denken aan tabellen met voertuigeigenschappen, geconstateerde gebreken of aan bijvoorbeeld dynamische parkeerdata. De RDW maakt het mogelijk om de data te doorzoeken met behulp van [SoQL queries](https://dev.socrata.com/docs/queries/). Daarnaast is ook het online inzien, visualiseren en downloaden van de gegevens mogelijk.

## Casus
Een politiemedewerker belt de RDW met de vraag om een lijstje met kentekens op te leveren die voldoen aan een bepaald profiel. Ze hebben een tip gekregen van iemand die een auto heeft zien staan bij een brandende 4G mast en willen graag contact met deze persoon zoeken. Er is echter een klein probleem: de beller heeft niet het gehele kenteken onthouden. Wel heeft hij een algemene omschrijving van de auto gegeven, als volgt:

> Het is al weer een paar dagen geleden, maar ik weet nog goed dat het een rode cabrio was die bij de zendmast stond. Het leek me een iets oudere auto, zeker wel tien jaar oud maar waarschijnlijk ouder. Volgens mij was het een Mazda? Of misschien toch een Opel? Ik ben niet zo goed met auto's. Van het kenteken heb ik wel een deel onthouden, maar exact weet ik het ook niet meer. Er kwam in elk geval een P in voor, en er zat geloof ik ook nog ergens NB in. Dat viel me toen op, omdat ik zelf ook een auto gehad heb met NB in het kenteken.

Wat zijn de kentekens van de voertuigen die voldoen aan het geschetste profiel?

## Voorbeelden met SoQL queries in de webbrowser

### Vraag alle gekentekende voertuigen op waarbij het voertuig meer dan 5 wielen heeft
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=aantal_wielen > 5`
##### Opmerking
Standaard krijg je maximaal 1000 rijen terug uit de API.

### Vraag alle gekentekende voertuigen op waarbij het merk begint met "OP"
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=merk like 'OP%25'`
##### Opmerking
Hier is in de URL het procentteken vervangen door %25, de URL-encoded versie van %.

​

### Vraag alle gekentekende voertuigen op waarbij de tweede kleur rood of blauw is
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=tweede_kleur = 'ROOD' or tweede_kleur = 'BLAUW'`
##### Opmerking
Het is ook mogelijk om AND en OR te gebruiken in je queries.

## Wist je dat
 - Medewerkers van het LIV (een verbond van RDW, politie en verzekeraars) regelmatig dit soort vragen binnenkrijgen?
 - Het is toegestaan om gegevens van de RDW open data te gebruiken voor particuliere en commerciele doeleinden, zolang je maar niet aangeeft dat de gegevens van de RDW komen? Meer info [hier](https://www.rdw.nl/over-rdw/dienstverlening/open-data/bijsluiter-open-data).
 - De RDW open data gegevens bevat over eerdere afkeurpunten en waarschuwingen bij een APK? Deze kan je bijvoorbeeld raadplegen bij het kopen van een nieuwe auto.
 - Er een fair use policy geldt voor het gebruik van de RDW open data zonder API key? Je kan alle data gewoon gebruiken, zonder dat je je hoeft aan te melden als developer.

​

​

English

 ---

# Burning towers

## Background
Like many other (semi-)governmental organizations, the RDW (the Dutch vehicle authority) has a large amount of [open data](https://opendata.rdw.nl/), which is accessible online. This data includes, among others, a table containing vehicle details and specifications, problems identified during a vehicles mandatory periodic check, and even dynamic parking data. The RDW allows people to access this data using [SoQL queries](https://dev.socrata.com/docs/queries/). Exploring, visualizing, and downloading this data is also possible.

## Case
A police officer calls the RDW with the request to provide a list of license plates that meet a specific profile. They have received a tip from someone who has seen a car near a burning 4G tower and would like to contact this person. However, there is a small problem: the caller did not remember the entire licence plate. However, he has given a general description of the car, as follows:

> It was a few days ago, but I clearly remember that I saw a red convertible near the transmission tower. It seemed like an older car, at least ten years old, but probably older. I think it could have been a Mazda? Or maybe an Opel? I'm not very good with cars. I can remember part of the license plate, but I don't remember it fully. In any case, it contained the letter P and I believe it also contained "NB". That stood out, because I used to have a car with "NB" in the license plate myself.

What are the license plates of the vehicles that meet the given profile?

## Examples of SoQL queries in a webbrowser

### Request a list of all vehicles that have more than 5 wheels
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=aantal_wielen > 5`
##### Note
By default, the API only returns 1000 rows.

### Request a list of all vehicles where the licence plate starts with "OP"
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=merk like 'OP%25'`
##### Note
In the URL, the percentage sign has been changed to %25, which is the URL-encoded version of the percentage sign.

​

### Request a list of all vehicles where the second color is either red (ROOD) or blue (BLAUW)
##### URL
`https://opendata.rdw.nl/resource/m9d7-ebf2.json?$where=tweede_kleur = 'ROOD' or tweede_kleur = 'BLAUW'`
##### Note
It is possible to use AND and OR in your SoQL queries.

## Did you know
 - Employees working at the LIV (a collaboration between the dutch police, the RDW, and insurance companies) regulary get questions like these?
 - That you're allowed to use the RDW's open data both privately and commercially, as long as you don't mention that the RDW provided the data? More info [here](https://www.rdw.nl/over-rdw/dienstverlening/open-data/bijsluiter-open-data) (in dutch).
 - That the RDW's open data can give you a list of found problems during a cars mandatory periodic checkup? You can use this if you ever want to buy a car in the Netherlands.
 - That there is a fair-use policy in place for the RDW's open data? This means that you can freely use it without having to register as a developer.

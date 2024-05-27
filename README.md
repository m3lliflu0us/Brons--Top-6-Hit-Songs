# Top 6 Hit Songs

Dit project bevat een interactieve lijst van de top 6 hit songs. De gebruiker kan liedjes aan de lijst toevoegen en de volgorde van de liedjes in de lijst wijzigen door ze te slepen.

## Code Uitleg

De code bestaat uit een HTML-bestand dat een lijst van liedjes weergeeft, en een JavaScript-bestand dat de functionaliteit van de lijst beheert.

### HTML

De HTML-structuur bestaat uit een `div` met de klasse "content", die een `ol` (geordende lijst) met het id "songList" bevat. Dit is waar de liedjes worden weergegeven. Er is ook een knop met het id "addSong" waarmee de gebruiker een nieuw liedje aan de lijst kan toevoegen.

### JavaScript

De JavaScript-code bevat een klasse genaamd `SongList`. Een instantie van deze klasse wordt gemaakt met het `ol`-element als argument. Deze klasse bevat de volgende methoden:

- `constructor(element)`: Deze methode initialiseert de `SongList` met een gegeven HTML-element en een array van liedjes.

- `render()`: Deze methode maakt de lijst van liedjes opnieuw aan op de webpagina. Het maakt ook de nodige event listeners voor het slepen van de liedjes.

- `addSong(song)`: Deze methode voegt een nieuw liedje toe aan de lijst en roept `render()` aan om de lijst bij te werken.

- `dragStart(e)`, `dragOver(e)`, `drop(e)`: Deze methoden beheren het slepen van de liedjes in de lijst. Ze worden aangeroepen wanneer de gebruiker begint met slepen, sleept over een ander liedje, en laat het liedje vallen, respectievelijk.

- `swapSongs(old_index, new_index)`: Deze methode verwisselt twee liedjes in de lijst op basis van hun indices.

Wanneer de "Add a Song" knop wordt geklikt, wordt de `addSong` methode aangeroepen om een nieuw liedje toe te voegen aan de lijst.

Tot slot wordt er een lijst van alle liedjes op de webpagina weergegeven.

#### Auteurs

- Bryce van der Werf
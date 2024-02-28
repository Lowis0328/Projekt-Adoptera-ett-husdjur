# Adoptera Husdjur
Detta projekt är en webbapplikation byggd med Flask, ett lättviktigt webbserverramverk för Python. Applikationen fungerar som en plattform för att adoptera husdjur, där användare kan bläddra igenom olika typer av husdjur (hundar, katter, kaniner) och se detaljerad information om varje husdjur.

Här är en detaljerad genomgång av vad vi har gjort i projektet:

Importera nödvändiga moduler: Vi importerar Flask-modulen och en hjälpmodul pets som innehåller information om husdjuren.

Skapa en Flask-app: Vi skapar en instans av Flask-klassen.

Definiera rutter (routes): Vi definierar flera rutter för vår app:

@app.route('/'): Detta är huvudsidan för vår app. Den visar en lista med länkar till olika typer av husdjur (hundar, katter, kaniner).

@app.route('/animals/<string:pet_type>'): Denna sida visar en lista med alla husdjur av en viss typ. pet_type är en variabel i rutten, vilket innebär att den kan vara vilken sträng som helst (i detta fall "dogs", "cats" eller "rabbits").

@app.route('/animals/<string:pet_type>/<int:pet_id>'): Denna sida visar detaljerad information om ett specifikt husdjur. pet_type och pet_id är båda variabler i rutten.

Skapa HTML-respons: För varje route genererar vi en HTML-respons som visar relevant information. Vi använder Python's f-string syntax för att infoga variabler direkt i HTML-koden.

Kör appen: Slutligen kör vi appen med app.run(). Vi sätter debug=True för att aktivera debug-läge, vilket gör att vi kan se detaljerade felmeddelanden om något går fel. Vi sätter också host="0.0.0.0" för att tillåta anslutningar från alla nätverksgränssnitt på servern.

Detta projekt är bra eftersom det lär oss grunderna i webbutveckling med Flask, inklusive hur man definierar rutter, genererar dynamisk HTML och hanterar HTTP-förfrågningar. Dessutom hjälper det oss att förstå hur webbapplikationer fungerar på en grundläggande nivå.

## Innehållsförteckning
1. [Projektinformation](#adoptera-husdjur)
2. [Installationsinstruktioner](#installationsinstruktioner)
3. [Teknologi](#teknologi)
4. [Funktioner](#funktioner)
5. [Licens](#licens)
6. [Bidragare](#Bidragare)

## Projektinformation
Detta projekt är en del av kursen [Webbserverprogrammering] vid [NTI Gymnasiet Örebro]. Projektet utfördes i tvån.

## Installationsinstruktioner
För att installera och köra detta projekt, följ dessa steg:

1. Klona detta repo till din lokala maskin med `git clone <https://github.com/Lowis0328/Projekt-Adoptera-ett-husdjur.git>`.

2. Navigera till projektets rotkatalog med `cd <project-directory>`.

3. Skapa en virtuell miljö med `python3 -m venv env`.

4. Aktivera den virtuella miljön med `source env/bin/activate` (för Linux/Mac) eller `.\env\Scripts\activate` (för Windows).

5. Installera de nödvändiga paketen med `pip install flask`.

6. Starta servern med `flask run`.

7. Öppna en webbläsare och gå till `http://localhost:5000` för att se applikationen.

## Teknologi

Detta projekt är byggt med följande teknologier:

- Flask
- Python
- HTML
- Python f-strings
- Dynamiska rutter

## Funktioner

Här är några av de huvudfunktioner som vår applikation erbjuder:

- Bläddra igenom olika typer av husdjur
- Se detaljerad information om varje husdjur
- Smidigt att implementera nya husdjur och ändra funktionen av programmet

## Licens

Detta projekt är licensierat under MIT-licensen. Se [LICENSE](LICENSE) för mer information.

## Bidgragare

- Lowe Granegärd
- Adam Khalid
- Zion Temo

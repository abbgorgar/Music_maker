# AI Projekt

#### I det här projektet så har jag gjort någonslags musik skapare AI. Det som den gör är att den kan skapa sina egna låter genom att tränna på andra och den kan också göra sina egna lyrics genom att träna på andra. Efteråt så skapar den två .mp3 filer en för låten och en för texten och på slutet ihopsätter båda .mp3 filerna och skapar en stor .mp3 fil med både låten och texten i den.

### Källor

#### Ideen för att skapa låten har jag fått från https://github.com/salu133445/musegan.
#### Och ideen för texten https://github.com/minimaxir/gpt-2-simple.

#### Min google colab länk https://colab.research.google.com/drive/1V9NjDummtaMQdQzzso9c7Ia0vJAGVkUF.
#### För att kunna använda colaben så måste man först koppiera det i sin egen gdrive. Också måste man ha __musgan__ mappen i sin gdrive

## Start

#### Från början så installerar man bibliotek och funktioner som ska användas. Det ska finnas fler bibliotek att instalera, men det kommer senare.
#### Efteråt så väljer man GPT-2 och instalerar. Storleken kommer att påverka både kvalite och hastighet.
#### Senare mountar med gdrive.

#### Därefter så kommer det tre separata delar. De första två kan köras utan varandra, men för att använda den sista så behöver man ha kört de första två innan.

## Part for music

#### I det här delen så genererar vi låten. 
* Man ska först och främs välja rätt mapp som man har instalerat innan.
* Därefter så ska man ladda ner förberedningsmateriale för att kunna tränna på den.
* Senare så kan man antigen köra på en redan trännat model eller tränna en egen.
#### För att köra på en redan tränat model måste man följa länken, ladda ner filen och sen lägga den i _musgan_ mappen.
https://docs.google.com/uc?export=download&id=19RYAbj_utCDMpU7PurkjsH4e_Vy8H-Uy
* Efter att man är klar med tränningen så kan man generera musik. Det kan göras på olika sätt och olika slags musik kan vara skapat. För att välja så behöver man gå in i mappen __exp/default/results/inference/__ och där kan man välja genre.
* Sist men inte minst skapar man .mp3 fil med själva låten. Man behöver göra det eftersom filerna skapas i .mid format.

## Part for text

#### För att kunna jobba med det här delen behöver man ha installerat GPT-2 från början.
* Först ska man markera rätt mapp där man jobbar.
* Sen väljer vi våran .txt fil där vi har våran text som AI ska tränna på. Om text filen är mindre än 10MB kan man bara dra den in i colab annars så måste man ha det i sin gdrive.
#### VIKTIGT! Text filen måste vara väl filtrerat dvs att man ska undvika meningar som återkommer många gånger och meningar som innehåller samma ord många gånger. Om man har flera låter så rekomenderar jag att della dem med en lång linje ---------- eller med uttryme men det fungerar bara om man har inte uttryme i själva låt texten.
* Därefter börjar man tränna modellen på valda text filen.
* Efteråt så kan man spara den tränning chekpointen i sin gdrive för att kunna använda den senare.
* Man kan också ladda upp redan trännat modell från gdrive och kära på den.
* Sen så blir det själva text genereringen och då när texten är skapat så får man en .txt fil där finns all text redan skriven.
* Och avslutningsvis så skapar vi en .mp3 tal från den .txt filen så vi genererade i förre punkten.

## Merge two .mp3 files together

#### Det man gör i det här delen är att man mergar ihop två sticken .mp3 filer. Det första av de är låten och den andra är lyrics.
#### Som sagt för att kunna göra det här steget så måste man ha gjort de första två innan.

# Reflektion 

## Det som var bra

#### Själva projektet gick som jag hade plannerat. Det fanns jättebra och enkla källor för allt och genom att leta länge så fick jag ett bra resultat. Det gick också jättebra att ändra koden som jag fick från källorna till min egen eftersom det var många grejer som passade inte eller fanns inte.

## Det som var mindre bra

#### Jag skulle vilja göra så att låten och texten passade till varandra och kanske ändra röstet som läser texten till en bättre för att just nu låter det lik som en robot.

### Om jag hade gjort om

#### Jag skulle konsentrerat mig mer på musik delen eftersom där fanns det mycket mer möjligheter än jag användde. Man kunde ha använt mer instrumenter och olika variationer av dem. 
#### Också jag tycker om man har allt det här som jag gjorde så blir det mycket enklare att försöka skapa riktigt musik som ska ha bra låt och text som är anpasad till den. 

# Vad har jag lärt mig?

#### Jag lärde mig nya modeller som GPT-2 och modeller som används i MuseGan. Jag har också lärt mig att omvandla olika fil typer till andra fil typer till exempel .mid till .mp3 eller .txt till .mp3.
#### Jag fick mer tid med Google Colab så nu känner jag mig säkrare där.

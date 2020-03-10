# AI Projekt

#### I det här projektet så har jag gjort någonslags musik skapare AI. Det som den gör är att den kan skapa sina egna låter genom att tränna på andra och den kan också göra sina egna lyrics genom att träna på andra. Efteråt så skapar den två .mp3 filer en för låten och en för texten och på slutet ihopsätter båda .mp3 filerna och skapar en stor .mp3 fil med både låten och texten i den.

#### Ideen för att skapa låten har jag fått från https://github.com/salu133445/musegan.
#### Och ideen för texten .....

#### Min google colab länk
#### https://colab.research.google.com/drive/1V9NjDummtaMQdQzzso9c7Ia0vJAGVkUF
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
* Sist men inte mins skapar man .mp3 fil med själva låten. Man behöver göra det eftersom filerna skapas i .mid format.

## Part for text


## Merge two .mp3 files together

#### Det man gör i det här delen är att man mergar ihop två sticken .mp3 filer. Det första av de är låten och den andra är lyrics.
#### Som sagt för att kunna göra det här steget så måste man ha gjort de första två innan.

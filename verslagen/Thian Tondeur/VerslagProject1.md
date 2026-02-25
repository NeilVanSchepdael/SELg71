### *NIET FINAAL*

# Verslag: SELab Opdracht 1

> Naam verslaggever: Thian Tondeur

## Beschrijving

We leren een package-manager te nuttigen, om het centraal beheer van geïnstaleerde software efficiënter te laten verlopen.

## Antwoorden op de vragen in de opdracht

#### Vraag 1 - De Bash-prompt toont de map/directory waar we ons nu bevinden. Wat is de naam van de directory waar je in terecht komt als je een Terminal-venster opent?
A: ```C:\WINDOWS\system32```

#### Vraag 2 - In welke map heb je het script bewaard?
   ```C:\Users\thian\onedrive\Documenten\1HOgent\SELab\Installatie.ps1```
A: --> In de SELab folder 

#### Vraag 3 - In welke map is het script bewaard in de screenshot onder stap 3?
   ```D:\Users\BertVV\Documents\HoGent\SELab\Installatie.ps1```
A: --> Ook in de SELab folder, maar op een andere drive.

#### Vraag 4 - Wat doen de opties -e en --id voor winget install?
A: -e: ID of Naam moet exact matchen. --id: Installeert exact pakket met specifiek ID



## Evaluatiecriteria

 - [ ] Je hebt een package manager voor jouw besturingssysteem geïnstalleerd.
 - [ ] Je hebt een script (PowerShell of Bash, afhankelijk van je besturingssysteem) geschreven en gebruikt om de opgesomde applicaties te installeren.
 - [ ] Je toont inzicht in de werking van een package manager en kan deze vlot kan gebruiken om basistaken uit te voeren.
 - [ ] Er is een verslag gemaakt op basis van het template.
 - [ ] Elk teamlid heeft de eigen cheat sheet aangevuld met nuttige commando's uit deze opdracht.
 - [ ] Je hebt GitHub correct geconfigureerd op je toestel en je hebt de basiscommando's (via CLI) in je vingers.
 - [ ] Er is een correct antwoord gegeven op de vragen die zijn aangeduid met een ❓.

## Problemen en oplossingen

### Probleem 1 - Kan GIT niet installeren via WinGet.

#### Input:
```PS C:\WINDOWS\system32> winget install git.git```
#### Output:
```   -                       
The `msstore` source requires that you view the following agreements before using.
Terms of Transaction: https://aka.ms/microsoft-store-terms-of-transaction
The source requires the current machine's 2-letter geographic region to be sent to the bac
kend service to function properly (ex. "US").

Do you agree to all the source agreements terms?
```
#### Einde Output

Ik kan geen input geven na de laatse regel, Geen "yes", geen "Y", geen Enter.
Hierdoor kan ik git niet installeren via WinGet.

## Voorbereiding demo

Beschrijf hier hoe je elk evaluatiecriterium zal demonstreren. Geef ook aan welke bestanden, commando's, enz. je zal gebruiken tijdens de demo.

## Reflecties

Maak werk van een degelijke reflectie over de opdracht.

Wat was moeilijk? Wat was eenvoudig? Wat hebben jullie geleerd van de opdracht? Wat zouden jullie anders doen als jullie het opnieuw moesten doen?

Als jullie nog andere opmerkingen hebben over de opdracht hebben, voel je vrij om ze te delen.

## Bronnen

Maak een lijst van alle bronnen die jullie hebben gebruikt tijdens het uitvoeren van de opdracht: boeken, handleidingen, HOWTO's, blog posts, enz. Citeer geen bronnen zoals ChatGPT of andere AI-tools rechtstreeks. Als je AI hebt gebruikt, laat het je dan leiden naar echte, betrouwbare bronnen in plaats daarvan.


### *NIET FINAAL*
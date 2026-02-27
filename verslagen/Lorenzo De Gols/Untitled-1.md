
# Verslag: SUBJECT

> Naam verslaggever: Lorenzo De Gols

## Beschrijving

Beschrijf de opdracht in eigen woorden. Wat werd er van jullie verwacht? Wat was het doel van de opdracht?
een packege manager installeren en gebruiken en een script schrijven voor dingen sneler te laten gaan 
## Antwoorden op de vragen in de opdracht
PS C:\Windows\system32> 

PS C:\Windows\system32> C:\Users\loren\Documents\installatie.ps1
PS C:\Windows\system32> C:\Users\loren\Documents\installatie.ps1

Voeg hieronder de antwoorden op de vragen in de opdracht toe. Gebruik voor elke vraag een aparte sectie.

### Vragen 

    ❓ De PowerShell-prompt toont de map waar we ons nu bevinden. Wat is de naam van deze directory? system 32
    ❓ In welke map heb je het script bewaard? bureaublad
    ❓ In welke map is het script bewaard in de screenshot onder stap 3? documents 
    ❓ Wat doen de opties -e en --id -e meot de naam exact overeen komen --id is er een package id 
Write-Host "Installatie algemene applicaties" -ForegroundColor Cyan

winget install -e --id Git.Git
winget install -e --id Mozilla.Firefox
winget install -e --id Adobe.Acrobat.Reader.64-bit
winget install -e --id GitHub.GitHubDesktop
winget install -e --id Microsoft.VisualStudioCode
winget install -e --id VideoLAN.VLC


Write-Host "Software voor System Engineering Lab" -ForegroundColor Yellow

winget install -e --id WinSCP.WinSCP
winget install -e --id Oracle.MySQLWorkbench

winget install -e --id Oracle.VirtualBox --version 7.2.2

winget pin add --id Oracle.VirtualBox
Hier beschrijf je het antwoord op de vraag. Voeg eventueel een screenshot, code snippets, enz. toe om je antwoord te ondersteunen. Als je veel code hebt, kun je linken naar een apart bestand in jullie repository (of ergens anders).

## Evaluatiecriteria

Kopieer de evaluatiecriteria uit de opdracht in deze sectie met behulp van een [task list](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists). Vink de criteria aan die jullie denken behaald te hebben. Geef een korte toelichting bij elk vakje dat jullie **niet** aangevinkt hebben.

De lijst hieronder is een voorbeeld. Vervang deze met de werkelijke evaluatiecriteria.

- [x] Het verslag is geschreven in Markdown
- [ ] De container draait
  - De container wou niet starten aangezien de Docker image niet gebouwd kon worden. Zie probleem 1 voor meer details.

## Problemen en oplossingen

Beschrijf hieronder eventuele problemen die jullie zijn tegengekomen tijdens het uitvoeren van de opdracht, met een korte beschrijving van wat er mis ging en hoe jullie het hebben opgelost (als het jullie gelukt is om het op te lossen). Als het niet gelukt is om het op te lossen, beschrijf dan hoe ver jullie zijn gekomen en wat jullie tegenhield om verder te gaan. Voeg eventuele foutmeldingen, screenshots, enz. toe.

Als jullie geen problemen zijn tegengekomen, schrijf dan "geen problemen ondervonden".

### Probleem 1 - Korte beschrijving van het probleem

Beschrijf hier het probleem uitgebreid met screenshots, code snippets, enz. en de oplossing die jullie al dan niet hebben gevonden.

## Voorbereiding demo

Beschrijf hier hoe je elk evaluatiecriterium zal demonstreren. Geef ook aan welke bestanden, commando's, enz. je zal gebruiken tijdens de demo.

## Reflecties

Maak werk van een degelijke reflectie over de opdracht.

Wat was moeilijk? Wat was eenvoudig? Wat hebben jullie geleerd van de opdracht? Wat zouden jullie anders doen als jullie het opnieuw moesten doen?
meer tijd voor de opdracht nemen en alles beter uitwerken van demos 
Als jullie nog andere opmerkingen hebben over de opdracht hebben, voel je vrij om ze te delen.

## Bronnen
https://learn.microsoft.com/en-us/windows/package-manager/winget/install
Maak een lijst van alle bronnen die jullie hebben gebruikt tijdens het uitvoeren van de opdracht: boeken, handleidingen, HOWTO's, blog posts, enz. Citeer geen bronnen zoals ChatGPT of andere AI-tools rechtstreeks. Als je AI hebt gebruikt, laat het je dan leiden naar echte, betrouwbare bronnen in plaats daarvan.


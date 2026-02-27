# Verslag: SEL-opdracht1

> Naam verslaggever: Tibo Dubois

## Beschrijving

Correct installeren van een package manager en leren een script correct op te stellen.

## Antwoorden op de vragen in de opdracht

Vraag 1 - De Bash-prompt toont de map/directory waar we ons nu bevinden. Wat is de naam van de directory waar je in terecht komt als je een Terminal-venster opent?

A: C:\WINDOWS\system32

Vraag 2 - In welke map heb je het script bewaard?

C:\Users\thian\onedrive\Documenten\1HOgent\SELab\Installatie.ps1 A: --> In de SELab folder

Vraag 3 - In welke map is het script bewaard in de screenshot onder stap 3?

D:\Users\BertVV\Documents\HoGent\SELab\Installatie.ps1 A: --> Ook in de SELab folder, maar op een andere drive.

Vraag 4 - Wat doen de opties -e en --id voor winget install?

A: -e: ID of Naam moet exact matchen. --id: Installeert exact pakket met specifiek ID

## Evaluatiecriteria

 - [x] Je hebt een package manager voor jouw besturingssysteem geïnstalleerd.
 - [x] Je hebt een script (PowerShell of Bash, afhankelijk van je besturingssysteem) geschreven en gebruikt om de opgesomde applicaties te installeren.
 - [ ] Je toont inzicht in de werking van een package manager en kan deze vlot kan gebruiken om basistaken uit te voeren.
   > WinGet functioneert niet, voor meer details zie probleem 1 en 2.
 - [x] Er is een verslag gemaakt op basis van het template.
 - [ ] Elk teamlid heeft de eigen cheat sheet aangevuld met nuttige commando's uit deze opdracht.
   > Niet elk teamlid heeft nuttige commando's gevonden voor hun cheatsheet.
 - [ ] Je hebt GitHub correct geconfigureerd op je toestel en je hebt de basiscommando's (via CLI) in je vingers.
 - [x] Er is een correct antwoord gegeven op de vragen die zijn aangeduid met een ❓.

## Problemen en oplossingen
 
Probleem 1 - Kan GIT niet installeren via WinGet.
Input:
PS C:\WINDOWS\system32> winget install git.git

Output:

<img width="462" height="116" alt="image" src="https://github.com/user-attachments/assets/37590ee7-bd0f-4776-9ed5-b60415955d6b" />


Einde Output
Ik kan geen input geven na de laatse regel, Geen "yes", geen "Y", geen Enter. Hierdoor kan ik git niet installeren via WinGet.

Oplossing 1 - Via andere lijn code probleem opgelost

Via deze lijn heb ik git wel kunnen installeren:

winget install -e --id Git.Git --accept-source-agreements --accept-package-agreements

## Reflecties

De opdracht was eerst lastig omdat ik onbekend met Winget was. Doordat ik de instructies van Github niet goed genoeg las was het niet makkelijker om de opdracht te voltooien. Ik zal beter Github lezen voor ik met opdracht start. Ik kan geen Git installeren via Winget dus kan


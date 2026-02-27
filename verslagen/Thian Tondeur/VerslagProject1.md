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

 - [x] Je hebt een package manager voor jouw besturingssysteem geïnstalleerd.
 - [x] Je hebt een script (PowerShell of Bash, afhankelijk van je besturingssysteem) geschreven en gebruikt om de opgesomde applicaties te installeren.
 - [ ] Je toont inzicht in de werking van een package manager en kan deze vlot kan gebruiken om basistaken uit te voeren.
   > WinGet functioneert niet, voor meer details zie probleem 1 en 2.
 - [x] Er is een verslag gemaakt op basis van het template.
 - [x] Elk teamlid heeft de eigen cheat sheet aangevuld met nuttige commando's uit deze opdracht.
 - [x] Je hebt GitHub correct geconfigureerd op je toestel en je hebt de basiscommando's (via CLI) in je vingers.
 - [x] Er is een correct antwoord gegeven op de vragen die zijn aangeduid met een ❓.

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

### Probleem 2 - kan het installatiescript niet uitvoeren.

#### Input:
```
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
```
#### Output:
```
PS C:\Windows\system32> Write-Host "Installatie algemene applicaties" -ForegroundColor Cyan

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

Installatie algemene applicaties

The `msstore` source requires that you view the following agreements before using.
Terms of Transaction: https://aka.ms/microsoft-store-terms-of-transaction
The source requires the current machine's 2-letter geographic region to be sent to the backend service to function properly (ex. "US").

Do you agree to all the source agreements terms?
```

## Voorbereiding demo
### Uitvoering DEMO:
  1. PowerShell ISE wordt geopend als administrator.
  2. We bypassen de execution policy met ```Set-ExecutionPolicy Bypass -Scope Process```, Hierdoor kunnen we scripts executeren. Dit geven we in in de CLI.
  3. We openen ons installatie script, en tonen aan hoe dit werkt. 
  ```
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
```
> Note: Pin zorgt dat deze applicatie niet automatisch mag geüpdate worden.
  

## Reflecties

#### Algemeen:
Uit onderstaande individuele reflecties blijkt dat de opdracht vooral moeilijk te begrijpen viel en er onvoldoende goed gepland was.

#### Thian:
Het was moeilijk de opdracht helemaal te begrijpen, qua overzichtelijkheid van de opdracht zelf. Problemen 1 en 2 zijn niet opgelost geraakt, omdat er geen error message      getoond wordt, waardoor het zoeken naar een mogelijkse oplossing zeer moeizaam doet verlopen. Er werd aan het einde van deze week geen oplossing gevonden.

Wat eerder eenvoudig was, was het schrijven van het verslag met MarkDown. Eerst waren daarbij problemen met de MarkDown text juist in GitHub geformateerd te krijgen, maar a.d.h.v. Visual Studio Code is dit toch goedgekomen.

#### Lorenzo:
Het moeilijkste aan deze opdracht was begrijpen wat er precies moest gebeuren en uitzoeken hoe alles werkte. Vooral Winget was moeilijk omdat ik daar nog niet veel ervaring mee had. Ik merkte ook dat ik de uitleg op GitHub beter had moeten lezen.

Een werkpunt voor mij is dus om eerst de uitleg goed te lezen voordat ik begin. Ook wil ik beter plannen zodat ik geen tijdsproblemen heb en rustiger kan werken.

Het makkelijkste deel was het verslag maken in Markdown. Dat ging vlot omdat dat duidelijk was voor mij.

#### Neil:
De opdracht was moeilijk omdat ik winget niet kon gebruiken. Ondanks op Windows 11 te werken en veel verschillende oplossingen te proberen + een leerkracht gemaild te hebben over mogelijke oplossingen is dit nog altijd niet gelukt.

#### Tibo:
De opdracht was eerst lastig omdat ik onbekend met Winget was. Doordat ik de instructies van Github niet goed genoeg las was het niet makkelijker om de opdracht te voltooien. Ik zal beter Github lezen voor ik met opdracht start.
#### Nathan:
In het begin vond ik deze opdracht moeilijk omdat ik veel moest opzoeken. Na alles eens gedaan te hebben werd het iets eenvoudiger en Markdown vond ik gemakkelijk. Toch heb ik nog wat moeite met het onthouden van de commando’s en moet ik daar nog op oefenen.

## Bronnen

#### Write-host commando leren aanpassen voor mooie onderscheidingen.
https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/write-host?view=powershell-7.5
#### WinGet installeren voor diegene waarbij dit nog niet geïnstalleerd was.
https://learn.microsoft.com/en-us/windows/package-manager/winget/install





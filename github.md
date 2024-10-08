{% include navbar_open.html %}
# Slik leverer du arbeidskrav på github:
Slik lager du et githubrepositorie, og dyttet arbeidet ditt til github. [Se også video](https://mediasite.uit.no/Mediasite/Play/facdd492ea4b4ceaa239fcfac56cd8941d) 

## Lage git-repositorie:
1. Lag en githubkonto (du trenger ikke bruke din uit-mail, det er valgfritt)
2. Gå inn i jupyter lab via terminalen ved å skrive `jupyter lab`, og åpne ny Terminal (+), og naviger dit du vil ha repositoriet på jupyter med `cd <mappenavn>` (se [tips og triks.md](https://github.com/uit-sok-1003-h24/notebooks/blob/main/tips_og_triks.md) for hvordan du navigerer i Terminal.) 
- *Alternativ til punkt 2.:* Logg på `jupyter.uit.no`, og åpne ny Terminal (+), og naviger dit du vil ha repositoriet på jupyter med `cd <mappenavn>` (se [tips og triks.md](https://github.com/uit-sok-1003-h24/notebooks/blob/main/tips_og_triks.md) for hvordan du navigerer i Terminal.) 
3. Konfigurer git med e-posten til kontoen og ditt brukernavn (bytt ut klammeparentesene med e-posten og brukernavnet til githubkontoen):
```
git config --global user.email "<e-post>"
git config --global user.name "<brukernavn>"
```
4. Gå til **Repositories**, trykk **New**, gi repositoriet et navn og velg **Private** eller **Public**. 
5. Hold denne fanen åpen, for du skal bruke html-adressen til denne siden.
6. Sørg for at du har et token. Gå eventuelt til [https://github.com/settings/tokens/new](https://github.com/settings/tokens/new) for å generere nytt token. *Hold fanen åpen for å ha tokenet tilgjengelig.*
7. kjør `git clone https://<token>@github.com/<sti>` der \<token\> er tokenet er det du fikk i 6. og \<sti\> er det som kommer etter **github.com/**  i html-adressen i 5.

 Du kan nå redigere repositoriet ditt
 
## Gi tilgang til faglærer/seminarleder
Du må også gi oss tilgang, slik at vi kan se repositoriet og arbeidet ditt. Det gjør du slik:

Når du er på nettsiden til repositoriet, gå til "Settings", og så "Manage access", og legg til "MarkusAase97". 
 
## Dytte repositoriet til github:
Dette gjør du ETTER at du har lagret en jupyter-fil i mappen til det klonede repositoriet. Sørg for at du lagrer i riktig mappe!

1. Naviger til repositoriemappen i Terminal (se [tips og triks.md](https://github.com/uit-sok-1003-h24/notebooks/blob/main/tips_og_triks.md) for hvordan du navigerer i Terminal.) 
2. Kjør i Terminal:
```
git add .
git commit -m "New repository"
git push 
```
Om du gjør endringer, og skal oppdatere repositoriet senere, kjører du samme prosedyre som over, men du kan endre teksten "New repository" til noe som beskriver oppdateringen.  

## Alternativ manuell løsning:
Hvis du sliter med å kjøre ting via terminal til repositorie kan dere følge følgende oppskrift:
1. Logg inn på dere egen bruker på [GitHub](github.com). 
2. Lag et repositorie, som f.eks. heter 'SOK-1003-eksamen-2024-mappe1' (mappe 1 innleveringen). (NB: Lurt å ha dette privat!)
3. Inne i repositorie, velg **Settings** og deretter **Collaborators and teams**.
4. Her gir du tilgang til følgende:
    - Dine gruppemedlemmer for mappe-oppgavene.
    - Fagansvarlig: 'MarkusAase97'
    - Læringsassistent: 'Jonazza'
5. Inne i repositorie kan du laste opp filer, som NoteBook'en (.ipynb fil), datasett (csv/xlsx) og eventuelle vedlegg.
6. Du laster opp ved å velge **Add file** og deretter **Upload files**. 
Oppdatering skjer ved å laste opp ny fil, og slette den forrige. Eller bruke git-kommandoer som nevnt over (push/add/commit) for å endre.

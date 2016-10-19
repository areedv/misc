Tjenesten “analyse og rapportering”: innledning
========================================================
author: Are, Nils, Tore
date: Sist oppdatert 19. oktober 2016

Møte i referansearkitekturgruppen, ehdir torsdag 20. oktober 2016


Disposisjon
========================================================

[1. Overordnet formål](#/for)

[2. Målgrupper og behov](#/mal)

[3. Gevinst og kostnad](#/gev)

[4. Eksisterende løsninger: muligheter og begrensninger](#/eks) 


1 Overordnet formål
========================================================
id: for
type: sub-section

Å kunne levere tilgang til data/informasjon på ulike nivå, det vil si i spennet fra grunnlagsdata til aggregerte, ferdig analyserte resultater, til ulike målgrupper (se [2 Målgrupper og behov](#/mal) under). I nivå som omhandler aggregering og analyse av data så kan også tjenesten levere dette interaktivt, altså at brukere selv kan plukke, sammenstille og behandle individuelle variabler som analyseres og visualiseres/presenteres av tjenesten.


1 a) Utfordringer ved interaktivitet og selvbetjening
========================================================

Omfattende krav til
- opplæring,
- dokumentasjon,
- styring (governance) og
- faglig kunnskap om grunnlagsdata


2 Målgrupper og behov
========================================================
id: mal
type: sub-section

|Målgruppe       |Behov|
|:---------------|:----|
|Helsearbeider   |Ferdige resultater fra enkeltregister (og sammenstilling på tvers av registre)|
|Helseleder      |Ferdige resultater fra enkeltregister og sammenstilling på tvers av registre|
|Myndighet       |Ferdige resultater fra enkeltregister og sammenstilling på tvers av registre|
|Pasient         |Ferdige resultater og grunnlagsdata (egne helseopplysninger) fra enkeltregister, ev også sammenstilling på tvers av registre (eksempelvis samtykke)|
_tabellen fortsetter på neste side_


2 Målgrupper og behov, forts.
========================================================

|Målgruppe       |Behov|
|:---------------|:----|
|Registerarbeider|Grunnlagsdata fra enkeltregister|
|Forsker         |Grunnlagsdata fra enkeltregister og sammenstilling på tvers av registre|
|Næringsliv      ||
|Innbygger mfl   |Ferdige resultater fra enkeltregister (og sammenstilling på tvers av registre)|


2 a) Eksempler på Behov
========================================================

Produkt:
- (kvalitets)indikatorer,
- helseatlas og
- datasett for videre/egen bearbeiding

Underliggende tjenester:
- grunnlagsdata,
- kobling,
- kryptering,
- analyse,
- presentasjon/visualisering +++


3 Gevins og kostnad
========================================================
id: gev
type: sub-section

|Gevinst|Kostnad|
|:------|:------|
|Helsearbeider gis grunnlag for *kvalitetsforbedring*|Krever data fra kvalitetsregistre, krever "streng" disiplin på innregistrering (god dekningsgrad), krever betydelige ressurser på analyse av grunnlagsdata|
|Helseleder gis grunnlag for *styring og kvalitetsforbedring*|Krever "streng" disiplin på innregistrering (god dekningsgrad), krever tilstrekkelig ressurser på analyse av grunnlagsdata, analyse med data fra flere registre er sårbar for "svakeste ledd"|
|Myndighet gis grunnlag for *prioritering*|Krever "streng" disiplin på innregistrering (god dekningsgrad), krever tilstrekkelig ressurser på analyse av grunnlagsdata, analyse med data fra flere registre er sårbar for "svakeste ledd"|
_tabellen fortsetter på neste side_


3 Gevins og kostnad, forts.
========================================================

|Gevinst|Kostnad|
|:------|:------|
|Pasient gis grunnlag for informert *valg av helsetjenester*|Krever data fra kvalitetsregistre, krever "streng" disiplin på innregistrering (god dekningsgrad), krever betydelige ressurser på analyse av grunnlagsdata, eksponering av helseopplysninger er "krevende" teknisk og juridisk|
|Forsker gis grunnlag for *kunnskapsproduksjon*|Eksponering av helse/pseudonyme opplysninger kan være "krevende" teknisk og juridisk, forvaltning av tidsbegrenset tilgang til data (tilbakekalling) må kunne håndteres, sammenstilling av data fra flere registre er sårbar for "svakeste ledd"|
|Næringsliv gis grunnlag for *forretningsutvikling*|Krever tilstrekkelig ressurser på analyse av grunnlagsdata, krever (muligens) "holdningsendring" mtp åpenhet og kommersiell utnyttelse av helsedata| 
|Innbygger mfl gis grunnlag for *generell informasjon*|Krever tilstrekkelig ressurser på analyse av grunnlagsdata|


4 Eksisterende løsninger: muligheter og begrensninger
========================================================
id: eks
type: sub-section

|Løsning                    |Mulighet/Begrensning|
|:--------------------------|:-------------------|
|FHI statistikkbanker       |Enkel fremstilling, liten/ingen (interaktiv) analysekapasitet|
|FHI intern resultattjeneste|?|
|HDir kvalitetsindikatorer  |Enkel fremstilling, liten/ingen (interaktiv) analysekapasitet, pt ikke skalerbar men omarbeides|
|HDir Dundas                |?|
|HDir NPR                   |Benytter/skal benytte Dundas?|
_tabellen fortsetter på neste side_


4 Eksisterende løsninger: muligheter og begrensninger, forts.
========================================================

|Løsning                    |Mulighet/Begrensning|
|:--------------------------|:-------------------|
|KREMT                      |Basert på R(Shiny), interaktiv analysekapasitet|
|Rapporteket                |Basert på Jasper Report Server og R, interaktiv analysekapasitet|
|MRS-R                      |Primært for registerdata fra MRS for presentasjon av kvalitetsindikatorer, basert på MS Power BI, tilbyr interaktiv analysekapasitet gjennom lokal klient, under utvikling per oktober 2016|

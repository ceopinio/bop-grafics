# 📊 BOP Gràfics

Aquest repositori d'R serveix per poder veure i aprendre el procediment de creació dels gràfics per als Baròmetres del Centre d'Estudis d'Opinió. L'arxiu utilitzat és de tipus `.Rmd`, que permet executar els codis dels gràfics un a un o tots alhora. L'script no inclou els gràfics de les estimacions electorals, que es poden trobar en el seu [repositori corresponent](https://github.com/ceopinio/ceo-estimacions/blob/main/src/report-figures.R).

## Estructura del repositori

-  📁 `src` conté el script de .Rmd utilitzat. Una breu descripció es [mostra a sota](#descripció-del-script).
-  📁 `dta` conté totes les dades d'entrada, com la base de dades del BOP corresponent, les dades de població, entre d'altres. Serà actualitzada cada vegada amb la nova matriu de dades. 
-  📁 `img` allotjarà les imatges generades pel script. 
-  📁 `config` inclou un fitxer `config.yaml` que defineix les variables de configuració que s'utilitzen a tot el codi com les rutes de les dades, els noms dels líders polítics, les dates dels BOP històrics, i els noms i colors dels partits. 

## Descripció dels scripts

L'script .Rmd conté diferents tipus de gràfics que s'inclouen en l'informe: de barres, dònut, lollipop, d'àrea, de línies temporals, entre altres. Algunes seccions que es mostren sota són constants entre els Baròmetres, per la qual cosa se n'inclou una descripció:

- 🌍 `Mostra` inclou els gràfics de l'informe que permeten verificar l'adequació de la 
mostra amb les dades poblacionals incloses en `poblacio.csv`. Aquí s'inclouen gràfics de sexe, nivell d'estudis, lloc de naixement, llengua primera i grups d'edat.
- 🗳️ `Electoral` inclou gràfics complementaris de la secció d'estimacions electorals, com l'evolució de les estimacions del CEO i la segona opció de vot segons intenció de vot. Les dades de l'evolució de les estimacions s'inclouen en `evolucio.csv`.
- 📢  `Líders` inclou els gràfics de l'informe de coneixement de líders, valoració de líders 
entre els qui els coneixen, entre els seus electors i entre els qui no ho són. 
- 💶  `Economia` inclou els gràfics de l'informe de situació econòmica actual de Catalunya 
i Espanya, situació retrospectiva, prospectiva i personal.
- 🤝  `Relacions Catalunya-Espanya` inclou els gràfics de l'informe de posicionament sobre la independència, tant actual 
com històric, preferència sobre la relació Catalunya-Espanya (històric), i actituds davant la independència.
- 🏛️ `Govern i institucions` inclou els gràfics de l'informe de valoració de la gestió dels Governs català i espanyol, i del grau de de satisfacció amb el 
funcionament de la democràcia, entre d'altres.

També s'inclouen les diferents seccions que canvien en cada BOP i que contenen els seus gràfics respectius.

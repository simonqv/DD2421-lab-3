# Hello!
This is the super cool readme of lab 3

## Assignment 3
### 1)
Det kan vara ett rimligt antagande om vi vet sedan innan att alla/nästan alla features är helt eller mestadels oberoende av varandra. Om vi dock inte vet detta eller vet att de är beroende av varandra så är det inte ett rimligt antagande. Men Naïve Bayes kan ändå fungera ganska bra på mer komplex (beroende) data pga. att man antingen kan klassifiera göra indelningar i features, eller att de tar ut varandra.

### 2)
*infoga bild*
Vi vet vad parametrarna motsvarar och vi kan anta att parametrarna inte är oberoende och bör därför använda en mer komplex/annan modell, t.ex. icke-Naïv Bayes. Vi kanske kan projecera datan in i ett annat space som är lättare separerbar (kanske tom. har större oberoende mellan featurersarna).


## Assignment 5
### 1)
Ja det är en förbättring. För att när vi har flera week klassifierare (ja det är så det stavas) (Vilket i vårat fall har relativt hög bias) och kombinerar reultaten med boosting så kan vi sänka biasen, där med få ett resultat som har en bättre avvägning mellan bias och varians.

### 2)
Skillnaden blir att den boostade k... har en mer komplex avvägning mellan klasserna en den icke boostade k....

### 3)
Ja, för att vi kan med boosting förbättra resultaten vi får av vår simplare modell utan att ta till en mer komplex modell. Men det är ingen garanti att den blir bättre.


## Assignment 6
### 1)
Ja det är en förbättring. Samma anledning som ovan. (d-tree kommer inte kunna bli särskilt djupa eftersom att vi bara har två parametrar så att det kommer bli en week k... med hög bias)

### 2)
Precis som innan blir den mer komplex.

### 3)
Återigen ja. Förmodligen skulle en mer complex modell kunna prestera bättre men vi kommer ganska bra undan med boosting i detta fall.


## Assignment 7
- **Outliers:** d-trees mer robusta mot outliers för att splitten/besluten försöker fånga så mycket data som möjligt (mycket information gain) och då blir påverkan av outliers liten. n-bayes påverkas mer av outliers än d-trees. Boosting kommer leda till ökan känslighet mot outliers, men vid våran testning så presterar ändå bootsing bättre än icke boosting i alla fall.

- **Irelevant features:** Varken n-bayes eller d-trees är speciellt känslig för irrelevanta features. Boosting shouldn't change this characeristic.

- **Predictive power:** d-trees have slightly higher or more or less the same predictive power as n-bayes, with or without boosting (depending on the data set).

- **Mixed types:** Det är lätt att hantera i både n-bayes och i d-trees, men är något mer prestandakrävande med n-bayes eftersom att vi behöver mer eller mindre räkna N olika modeller för de N olika data typera och sedan multiplicera sannorlikheterna. Medans med d-tree kan vi hantera allt i ett och samma träd, dock så hanter d-trees inte continues featues lika bra som n-bayes (stämmer inte riktigt överens med vad vi har sett). Boosting should not change this characteristic.

- **Scalability:** n-bayes scales well over high dimentional data thanks to the feature independence assumption and requires a relative low amount of data to train. d-trees can grow quite complex in high dimentional data.

Vi skulle i första hand välja en boosted modell för att den verkar alltid prestera bättre med dessa modeller och för att den inte har någon direkt negativ inverkan på någon av kriterierna. Over all verkar det vara ganska jämnt d-trees och n-bayes emellan med sina egna pros och cons, men vi skulle välja att använda oss av d-trees för att de verkar i våra fall prestera bättre. Slutsatsen blir alltså en boosted ensamble av d-trees.

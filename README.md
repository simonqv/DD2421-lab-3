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



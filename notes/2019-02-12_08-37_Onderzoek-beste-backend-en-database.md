---
tags:
  - Afstuderen
  - Argumentatie
  - Initialisatie- en onderzoeksfase
  - Onderzoek
  - Portfolio
---
### Onderzoek
> Onderzoeksstrategie: Bieb 

## API / Backend talen
Om wat zwaardere taken te doen en te verbinden met een database wordt er een API ontwikkeld waar de mobiele applicatie verbinding mee maakt. Er zijn een hoop talen waarin een API geschreven kan worden. Deze worden vergeleken met elkaar. Om een begin selectie te maken van talen waar naar gekeken gaat worden, is er besloten dat er een lijstje wordt gemaakt waar de opdrachtnemer in ieder geval een basiskennis van heeft en wat gebruikt kan worden om een restful api te schrijven. Daar zijn de volgende talen en frameworks uitgekomen:

-   JavaScript in combinate met Express.js (node)
-   Python in combinatie met Django 
-   C# in combinatie met ASP.NET Core
-   Java in combinatie met Spring Boot

### Belangrijke elementen bij het kiezen van een web framework
De onderstaande elementen gelden in principe bij het kiezen van elke programmeer taal of framework.

- Inspanning om het te leren: als frameworks redelijk gelijk zijn en de klant stelt geen eisen aan een web framework, dan is het vanzelfsprekend om te kiezne voor het web framework waar de ontwikkelaar(s) al de meeste kennis over heeft / hebben.
- Productiviteit: hoe snel kunnen nieuwe functionaliteiten ontwikkeld worden en fouten uit de code gehaald worden. Hierbij moet gekeken worden naar het doel van de framework, de beschikbare libraries en of het framework best practices hanteert. 
- Prestatie: voor de meeste projecten niet het belangrijkst aangezien bijna alle veel gebruikte frameworks en talen snel genoeg zijn voor de meeste toepassingen. 
- Support voor caching: welk framework heeft de beste (stnadaard) support voor caching. 
- Schaalbaarheid: welk framework is het meest geschikt voor schalen, zowel horizontaal als verticaal.
- Beveiliging: welk framework heeft de beste (standaard) support voor web beveiliging. 

 > Bron: https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Web_frameworks

### Vergelijkingen
| Taal                           | Inspanning om te leren | Productiviteit | Prestatie | Support caching | Schaalbaarheid | Beveiliging |
| ------------------------------ | ---------------------- | -------------- | --------- | --------------- | -------------- | ----------- |
| Javascript (Express.js / node) | +-                     | +              | ++        | +-              | +-             | +-          |
| Python (Django)                | +-                     | ++             | +-        | +-              | ++             | ++          |
| C# (ASP.NET Core)              | ++                     | ++             | +         | +-              | ++             | ++          |
| Java (Spring Boot)             | +                      | +              | +         | +-              | +              | +           |

- Javascript: 3.5
- Java: 3,83
- Python: 4
- C#: 4.5

Zoals in deze tabel te zien is, komen Django en ASP.NET Core het best uit het onderzoek. Deze gaan we aan de hand van de verwachte requirements met elkaar vergelijken.  
 > Bron: https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Web_frameworks 

 > https://medium.com/@OPTASY.com/how-to-scale-your-node-js-app-best-strategies-and-built-in-tools-for-scalability-a1725df082f5

 > https://medium.com/@mihaigeorge.c/web-rest-api-benchmark-on-a-real-life-application-ebb743a5d7a3

 > https://hunter2.com/how-secure-are-popular-web-frameworks-comparing-options

 > https://medium.com/the-node-js-collection/why-the-hell-would-you-use-node-js-4b053b94ab8e

 > https://djangobook.com/scaling-django/

 > https://docs.microsoft.com/en-us/dotnet/standard/modern-web-apps-azure-architecture/common-web-application-architectures

### Python (Django) vs C# (ASP.NET Core)
De volgende twee lijsten laten zien waar beide talen / frameworks in uit springen. 

Python in combinatie met Django:
- AI / ML toepassingen (handig voor eventuele toepassingen in de app)
- Veel out of the box libraries
- Erg snelle ontwikkeling (handig voor PoC)

C# in combinatie met .NET Core:
- Strongly typed waardoor er minder fouten gemaakt worden en minder getest hoeft te worden
- Containarizing van microservices
- Inspanning om te leren (persoonlijk)
- Snelheid
- Realtime data mogelijkheden (signal r)

Beide erg goed:
- Community
- Documentatie
- Beveiliging 

### Argumentatie gemaakte keuze
Uiteindelijk komt de keuze terrecht op C# in combinatie met .NET Core. Hier is uiteindelijk voor gekozen omdat C# een aantal sterke punten heeft die Python niet heeft en de sterke punten van Python ook opgevangen kunnen worden door C#. Vaak wordt Python gezien als leider in de AI / ML wereld, echter heeft .NET tegenwoordig een ML.NET framework welke naar verwachting meer dan genoeg mogelijkheden biedt voor eventuele AI / ML functies in de app. Daarnaast geldt dat Django handig is voor een snelle ontwikkeling, maar doordat er al veel voorkennis is van C# en .NET Core is er de verwachting dat dat weinig verschil gaat maken. De goede documentatie over microservices en containarizing in combinatie met realtime mogelijkheden en dat C# strongly typed is heeft de keuze op .NET Core doen laten vallen voor de API.  

## Database
Voor het opslaan van data in de cloud gaat een externe database gebruikt worden. Ten eerste gaat er gekeken worden of er een relationele database nodig is of een NoSQL database. Aan de hand van dit resultaat wordt er gekeken naar 2 of meer databases binnen deze groep. 

### NoSQL of relationele database
NoSQL:
- Flexiebel: als er veel verandering in de modellen plaats vindt, dan kan dit makkelijk opgevangen worden door het gebruik van een NoSQL database.
- Mogelijke horizontale schaling ten opzichte van verticale schaling. 
- Concurrent prestaties: NoSQL gebruikt locked transactions ipv een locking mechanisme waardoor er geen ander proces gebruik kan maken van de database tot dat de         transactie voltooid is wat handig is als er veel gebruikers tegelijkertijd gebruik moeten maken van de app.

Rlationele database:
- Volwassen waardoor er veel minder verandering plaats vindt. 
- Handig voor complexe queries en complexere datasets die vast staan

Hierdoor gaat er in dit project gewerkt worden met een NoSQL database. Dit omdat nog niet alle eisen vast staan en er tijdens het project nog veel kan veranderen. Zeker in versie 2 van het project (na Paaspop) kan er nog veel veranderen waardoor NoSQL een geschikt database model is. Daarnaast moet het in principe geschikt zijn om gebruikt te worden door veel bezoekers in één keer waar de mogelijkheid tot horizontale schaling en conccurent prestatie erg fijn zijn. 

 > bron: https://resources.whitesourcesoftware.com/blog-whitesource/when-to-consider-a-nosql-vs-relational-database
 
 > https://medium.com/xplenty-blog/the-sql-vs-nosql-difference-mysql-vs-mongodb-32c9980e67b2

### Vergelijking NoSQL database omgevingen 
Er zijn twee eisen voor de NoSQL database die gekozen kan worden. Dit zijn dat de database drivers en een library heeft voor .NET Core en dat het een Key-Document structuur heeft. Een Key-Document structure is van belang omdat er OO geprogrammeerd gaat worden en er objecten opgeslagen moeten kunnen worden in een database. Hierdoor zijn er twee database omgevingen overgebleven namelijk: MongoDB en Couchbase.  
De enige eis is dat de gekozen NoSQL database drivers en een library heeft voor .NET Core. Dit is namelijk het gekozen backend framework. 

|                                 | MongoDB                                   | couchbase                 |
| ------------------------------- | ----------------------------------------- | ------------------------- |
| Community                       | X                                         |                           |
| Supported programming languages | X                                         |                           |
| Indexing                        | X (Old reliable B-Tree vs new Skip Lists) |                           |
| Server-side scripts             | Javascript                                | View functions Javascript |
| Configuration optiones          |                                           | X                         |


 > bron: https://stackshare.io/stackups/couchbase-vs-mongodb-vs-mysql

 > https://db-engines.com/en/system/Couchbase%3BMongoDB

 > https://dzone.com/articles/mongodb-vs-couchbase-part-2-json-tooling-and-more

### Argumentatie voor de gemaakte keuze
Voor de database gaat er in dit project gebruik gemaakt worden vna MongoDB. Dit omdat het een grote community heeft, een goede intergratie met .NET Core en een Key-Document structuur database omgeving is.
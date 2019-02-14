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

## Cross platform mobile app development frameworks
De eis van Paaspop is dat er een cross platform app ontwikkeld moet worden (een app die zowel draait op Android als IOS) omdat ze geen bezoekers uit willen sluiten. 
Er is gekeken naar mogelijke frameworks en hier zijn drie kandidaten uit gekomen op basis van kennis van de opdrachtnemer en de populairiteit van het framework. Dit zijn:
1. Reacht Native (Javascript)
2. Xamarin (C#)
3. Flutter (Dart)

## Vergelijkingen
### Xamarin
Xamarin is overgenomen door Microsoft en dient nu als framework in de .NET omgeving waar door middel van C# een mobiele app gemaakt kan worden. 
Voordelen van xamarin:
- Prestaties zijn vergelijkbaar met native apps. 
- Veel integratie met native hardware componenten.
- Xamarin.Forms waarmee je UI code kunt ontwikkelen voor zowel Android als IOS. 
- Offline support

Nadelen van xamarin:
- Overhead.
- Ondanks Xamarin.Forms nog steeds relatief veel tijd in UI development.
- Een app wordt erg groot.
- Kost wat tijd voor de opdrachtnemer om dit te leren.
- Relatief weinig componenten en 3rd party libraries. 
- Niet echt een community 

### React Native
React Native is ontwikkeld door Facebook en gebruikt Javascript in combinatie met het React Framework om een cross platform app te kunnen ontwikkelen.
Voordelen van React Native:
- Een Native UI.
- Op klein niveau stukken code los van elkaar zodat veel herbruikt kan worden en het flexibel is.
- Heel erg veel componenten en libraries die beschikbaar zijn.
- Hot reloading.
- Grote community

Nadelen van React Native:
- Prestatie doordat er een javascript laag tussen de react applicatie laag en hardware componenten zit. 
- Niet ideaal voor enorm ingewikkelde applicaties.
- Opstarten van de app duurt wat langer. 
- Heeft wat nadelen met betrekking tot navigatie. 

### Flutter
Flutter is ontwikkeld door Google en gebruikt Dart als programmeertaal. Deze taal is bij de opdrachtnemer nog onbekend maar het is een OO taal die makkelijk te leren is.
Voordelen van Flutter:
- Functies kunnen snel gemaakt worden. 
- Widgets zijn erg gebruik vriendelijk en kunnen makkelijk aangepast worden. 
- Goede prestaties.
- Hot reload.

Nadelen van Flutter:
- Nog niet heel erg volwassen.
- weinig 3rd party libaries. 
- Grote van de app.
- Nog geen support voor CI.

### Xamarin vs React Native vs Flutter

|                                         | Xamarin | React Native | Flutter |
| --------------------------------------- | ------- | ------------ | ------- |
| Learning curve                          | +-      | +            | +-      |
| Prestaties                              | ++      | +-           | +       |
| Productiviteit                          | +-      | ++           | +       |
| Native UI                               | +-      | +            | +       |
| Architectuur                            | +-      | +            | +       |
| Community                               | -       | ++           | +       |
| 3rd party libraries / ready componenten | +-      | ++           | +-      |
| Gebruik door grote bedrijven            | -       | ++           | +-      |
| Volwassenheid van het framework         | ++      | ++           | +-      |
| Documentatie                            | ++      | +            | ++      |

Xamarin: 3.4
Flutter: 3.7
React Native: 4.4

### Argumentatie gemaakte keuze
Voor dit project gaat er gewerkt worden met React Native om een cross platform te ontwikkelen. Hiervoor is gekozen door de volwassenheid van het framework in combinatie met de community en beschikbare 3rd party libraries. Daarnaast heeft de opdrachtnemer hier ook al een beetje kennis van waardoor er snel op een goede manier een POC ontwikkeld kan worden.

> Bron: https://hackernoon.com/flutter-vs-react-native-vs-xamarin-for-cross-platform-development-5f92cfb178ff

> https://www.netsolutions.com/insights/flutter-vs-react-native-vs-xamarin-which-framework-is-right-for-you/
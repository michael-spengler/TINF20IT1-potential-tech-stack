# TINF20IT1 Blockchain & Moderne Konzepte
Die in diesem Repo gesammelten Komponenten für einen möglichen "Tech Stack" können sowohl im Spezialgebiet Blockchain Technologie als auch insgesamt unter dem Stichwort Moderne Konzepte hilfreich sein.


## Projektüberblick
| Name         | Projekt Blockchain     | Projekt Moderne Konzepte |
|--------------|-----------|------------|
| Edin Music |   https://github.com/NoohDoor/SnakeCoin    | https://github.com/NoohDoor/ModerneKonzepteTrust        |
| Lukas Michalek |   https://github.com/NoohDoor/SnakeCoin    | https://github.com/NoohDoor/ModerneKonzepteTrust        |
| Johnny Wedel |  https://github.com/NoohDoor/SnakeCoin | | 
| Jan Philip Werthmann |  https://github.com/NoohDoor/SnakeCoin | https://github.com/FigurDesign/UnitConverter.git | 
| Moritz Bartenbach | https://github.com/NoohDoor/SnakeCoin | https://github.com/FigurDesign/UnitConverter.git | 
| David Schwab |  https://github.com/NoohDoor/SnakeCoin | | 
| Tobias Winkler |   | https://github.com/0x7477/DonationSimulator | 
| Louis Dorweiler | https://github.com/Ethernol/C2H6O | https://github.com/russiankidgohax/MarxCoin |
| Simon Spielmann | https://github.com/Ethernol/C2H6O | |
| Jörn Vaupel | https://github.com/Ethernol/C2H6O | |
| Pascal Fitzner | https://github.com/Ethernol/C2H6O | |
| Luca Tiedemann | https://github.com/techsupport-noah/ChainOfTrust | | 
| Belana Roman | https://github.com/techsupport-noah/ChainOfTrust | | 
| Noah Wiederhold | https://github.com/techsupport-noah/ChainOfTrust | | 


## Vorläufige Punktevergabe und Feedback
| Projekt      | Übriggebliebene Anregungen / Feedback     | Vorläufige Punktevergabe von 100 |
|--------------|-----------|------------|
| [SnakeCoin](https://github.com/NoohDoor/SnakeCoin) (Blockchain) | Super Thema. Ausdauernd umgesetzt. Mehr Links und oder Screenshots in der Readme wären hilfreich für Besucher und mögliche Contributors. Den "About" Text im Repo definieren (rechts oben im Repo)    | 93        |
| [Ethernol](https://github.com/Ethernol/C2H6O)  (Blockchain) | Screenshots in der Readme - welche den Sinn und Zweck der Applikation beschreiben - wären hilfreich für Besucher und mögliche Contributors. Zusätzlich wäre hilfreich für den Leser warum welche Technologie wofür gewählt wurde. Den "About" Text im Repo definieren (rechts oben im Repo) - Fortschritt siehe https://github.com/Ethernol/C2H6O/issues/4  | 91        |
| [Chain Of Trust](https://github.com/techsupport-noah/ChainOfTrust)  (Blockchain) | Herausforderndes Thema ausdauernd umgesetzt (trotz extrem vieler Herausforderungen im Hinblick auf noch nicht ausgereifte web3 Werkzeuge). Screenshots in der Readme wären hilfreich für Besucher und mögliche Contributors. Den "About" Text im Repo definieren (rechts oben im Repo)    | 94        |
| [Trust](https://github.com/NoohDoor/ModerneKonzepteTrust) (Moderne Konzepte) | Cooles Thema. Angemessener Umfang bezüglich der Implementierung.   | 92        |
| [Unit Converter](https://github.com/FigurDesign/UnitConverter.git) (Moderne Konzepte) | Cooles Thema. Angemessener Umfang. Wertvolle Open Source Assets. Optimierungspotentiale (Low hanging fruits): https://github.com/FigurDesign/UnitConverter/issues/2    | 93        |
| [Donation Simulator](https://github.com/0x7477/DonationSimulator) (Moderne Konzepte) | Spannendes Thema. Gut und ausdauernd umgesetzt. (Zusätzliche) Screenshots der web app innerhalb der readme oder ein link auf die "deployte" web app an sich wäre m.E. perfekt um anhand der readme noch schneller zu checken wie genau die web app aussieht und benutzt werden kann. Details siehe: https://github.com/0x7477/DonationSimulator/issues/1     | 96 (1,2)        |
| [Marx Coin](https://github.com/russiankidgohax/MarxCoin) (Moderne Konzepte) | Sehr ganzheitliche und gleichzeitig in einigen Bereichen fokussierte Erkundung innovativer web3 Themen. Sehr ausdauernd erkundet und umgesetzt.    | 99 (1,0)       |

## Genutzte Punktetabelle
https://github.com/michael-spengler/DHBW-Wissenschaftliche-Arbeiten/blob/main/Punkte-Noten-Tabelle%202022.pdf


## Blockchain Programming Stack Demo
In this context we drafted a censorship resistant chat platform. This served as conceptual and technological inspiration for the individual projects designed and implemented by the students - see overview above.

## In General
### Decentralized vs. Centralized Paradigms
Not your keys - not your crypto.

## Frontend
### Learning Goals
Explore and leverage [TypeScript](https://www.typescriptlang.org/) and [svelte](https://svelte.dev/).
We use [TypeScript](https://www.typescriptlang.org/) as Programming Language.  
We use [svelte](https://svelte.dev/) because it seems to combine best of angular, vue and react. See also [svelte + web3 interaction example](https://github.com/App-Entwicklung/frontend-svelte/blob/main/src/App.svelte)  

**Alternativen** 
Im Hinblick auf "Native Apps" kann https://flutter.dev interessant sein. Wobei die web3 Anbindung in diesem Kontext erfahrungsgemäß aktuell (noch) sehr [herausfordernd](https://github.com/App-Entwicklung/frontend/blob/main/lib/helpers/contract.dart#L46-L75) ist. 

### Details
To start the frontend locally enter:  
```
cd frontend/our-first-svelte-app
trex run start
```


## Off Chain Backend
### Learning Goals
Explore and leverage [TypeScript](https://www.typescriptlang.org/) and [deno](https://deno.land).

### Details
The Off Chain Backend is not needed for the actual application. I only include this for demo reasons which might be helpful e.g. in case some of the students need an off chain backend.

## On Chain Backend
### Learning Goals
Explore and leverage browser wallets like metamask.  
Explore and leverage solidity (very basics).    
Explore and leverage the web3 online IDE [remix.ethereum.org](https://remix.ethereum.org).  

### Details
The following smart contract can be used to test things:  
https://goerli.etherscan.io/address/0x86bb1F3B75b013a1Bdd31EFb20de79E20b137036


It has been deployed via [this transaction](https://goerli.etherscan.io/tx/0xf20e541f2f38ae85db00903baefd1ea012f95564d4347e52b902e605a41b63c6).  

 



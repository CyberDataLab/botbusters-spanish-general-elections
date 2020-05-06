# Process of data collection

The following document reports the supplementary material for the process of data collection, as described in [![Preprint](https://webs.um.es/mattia.zago/images/BB10N-Badge-ArXiV.svg)](https://arxiv.org/abs/2004.00931). 

## Parameters

### Observation period

- Start date: 2019-10-04
- End date: 2019-11-11

Relevant dates:
- October 10th, 2019 — Santiago Abascal (VOX’s political leader) participated in the live TV show “El Hormiguero”
- October 19-20th, 2019 — Riots in Catalonia
- October 24th, 2019 — Exhumation of Francisco Franco
- November 4th, 2019 — Electoral debate on national TV
- November 10th, 2019 — General election day

### Queried hashtags

A total of 46 hashtags have been used to query the Twitter APIs.

| Group      | Keyword                    || Group        | Keyword                    |
| :---       | :---:                      | --- | :---    | :---:                      |
| VOX        | `#VOX`                     || PSOE         | `#AhoraSì`                 |
| VOX        | `#EspañaSiempre`           || PSOE         | `#AhoraEspaña`             |
| PP         | `#PartidoPopular`          || PSOE         | `#PSOE`                    |
| PP         | `#PP`                      || PSOE         | `#PSOEcompraVotos`         |
| PP         | `#PorTodoLoQueNosUne`      || Elections    | `#10N`                     |
| Ciudadanos | `#Cs`                      || Elections    | `#10NElecciones`           |
| Ciudadanos | `#Ciudadanos`              || Elections    | `#10Noviembre`             |
| Ciudadanos | `#EspañaEnMarcha`          || Elections    | `#Elecciones10N`           |
| UP         | `#ElPoderDeLaGente`        || Elections    | `#eleccionesgenerales10N`  |
| UP         | `#MamadasPodemos`          || Elections    | `#EleccionesNoviembre2019` |
| UP         | `#SePuede`                 || Exhumation   | `#exhumacionFranco`        |
| UP         | `#UnGobiernoContigo`       || Exhumation   | `#francisfrancoesp`        |
| UP         | `#UnidasPodemos`           || Exhumation   | `#FrancoCalientaQueSales`  |
| Catalonia  | `#116YA`                   || Exhumation   | `#unboxingfranco`          |
| Catalonia  | `#disturbiosBarcelona`     || Debate       | `#Debate10N`               |
| Catalonia  | `#EstadoDeExcepcion`       || Debate       | `#DebateA5`                |
| Catalonia  | `#MarlaskaDimisionYa`      || Debate       | `#Debatea7RTVE`            |
| Catalonia  | `#SpainIsAFascistState`    || Debate       | `#DebateElectoral`         |
| Catalonia  | `#ThisIsTheRealSpain`      || Debate       | `#DebatePresidencial`      |
| Catalonia  | `#tsunamidemocractic`      || Debate       | `#ElDebate4N`              |
| Catalonia  | `#tsunamiinfiltrado`       || Debate       | `#ElDebateEnRTVE`          |
| AbascalEH  | `#SantiagoAbascalEH`       || Debate       | `#UltimaOportunidadL6`     |
| AbascalEH  | `#elhormigueroabascal`     || AbascalEH    | `#BoicotElHormiguero`      |

### Bag of words

Here follows the complete list of keyword used to create the bag of words. Since the data have been anonymized, we are not including the list of usernames of verified political accounts. The code to generate the complete list is available on [Phase 2 Notebook (Verified political party regex definitions)](../notebooks/Phase2.ipynb#Verified-political-party-regex-definitions).

| Group      | Keyword                 || Group        | Keyword                     |
| :---       | :---:                   | --- | :---    | :---:                       |
| VOX        | `VOX`                   || PP           | `PartidoPopular`            |
| VOX        | `EspañaSiempre`         || PP           | `Partido Popular`           |
| VOX        | `Abascal`               || PP           | `PP`                        |
| VOX        | `Santiago Abascal`      || PP           | `PorTodoLoQueNosUne`        |
| VOX        | `Santi Abascal`         || PP           | `Pablo Casado`              |
| Ciudadanos | `Ciudadanos`            || PSOE         | `AhoraSì`                   |
| Ciudadanos | `\#Cs`                  || PSOE         | `AhoraEspaña`               |
| Ciudadanos | `EspañaEnMarcha`        || PSOE         | `PSOE`                      |
| Ciudadanos | `Albert Rivera`         || PSOE         | `PSOEcompraVotos`           |
| Ciudadanos | `Rivera`                || PSOE         | `Pedro Sánchez`             |
| UP         | `UnidasPodemos`         || Elections    | `10N`                       |
| UP         | `Unidas Podemos`        || Elections    | `10NElecciones`             |
| UP         | `ElPoderDeLaGente`      || Elections    | `10Noviembre`               |
| UP         | `MamadasPodemos`        || Elections    | `Elecciones10N`             |
| UP         | `SePuede`               || Elections    | `eleccionesgenerales10N`    |
| UP         | `UnGobiernoContigo`     || Elections    | `EleccionesNoviembre2019`   |
| UP         | `Pablo Iglesias`        || Exhumation   | `exhumacionFranco`          |
| Catalonia  | `116YA`                 || Exhumation   | `francisfrancoesp`          |
| Catalonia  | `disturbiosBarcelona`   || Exhumation   | `FrancoCalientaQueSales`    |
| Catalonia  | `EstadoDeExcepcion`     || Exhumation   | `unboxingfranco`            |
| Catalonia  | `MarlaskaDimisionYa`    || Debate       | `Debate10N`                 |
| Catalonia  | `SpainIsAFascistState`  || Debate       | `DebateA5`                  |
| Catalonia  | `ThisIsTheRealSpain`    || Debate       | `Debatea7RTVE`              |
| Catalonia  | `tsunamidemocractic`    || Debate       | `DebateElectoral`           |
| Catalonia  | `tsunamiinfiltrado`     || Debate       | `DebatePresidencial`        |
| AbascalEH  | `SantiagoAbascalEH`     || Debate       | `ElDebate4N`                |
| AbascalEH  | `elhormigueroabascal`   || Debate       | `ElDebateEnRTVE`            |
| AbascalEH  | `BoicotElHormiguero`    || Debate       | `UltimaOportunidadL6`       |

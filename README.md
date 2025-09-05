# Projekt Banka: Moderný Návrh Bankového Systému v Jave

## O Projekte

Tento projekt je praktickou ukážkou a cvičením v návrhu flexibilného a rozšíriteľného systému pre správu bankových
účtov. Cieľom je vytvoriť jadro bankovej aplikácie, ktorá dokáže spravovať rôzne typy produktov (osobné účty, firemné
účty) s odlišnými pravidlami, poplatkami a dátovými požiadavkami.

Hlavný dôraz nie je kladený na komplexnú business logiku, ale na kvalitu, čistotu a udržateľnosť softvérového návrhu s
využitím moderných princípov a techník v jazyku Java.

Technologické Ciele a Princípy
Počas vývoja tohto projektu sa budeme riadiť a učiť nasledujúce koncepty:

**Jazyk**: Java 17+ (s využitím moderných prvkov ako record)

**Základný Princíp**: Kompozícia nad dedičnosťou (Composition over Inheritance) – vyhneme sa rigidným hierarchiám tried
a budeme skladať objekty z menších, znovupoužiteľných komponentov.

### SOLID Princípy:

- S - Single Responsibility Principle
- O - Open/Closed Principle
- L - Liskov Substitution Principle
- I - Interface Segregation Principle
- D - Dependency Inversion Principle

Návrhové Vzory (`Design Patterns`): Prakticky si ukážeme použitie vzorov ako:
- `Strategy`
- `Factory / Abstract Factory`
- `Builder`
- `Observer`

Čistý Kód (`Clean Code`): Dôraz na čitateľnosť, jednoduchosť a expresívnosť kódu.

### Štruktúra Projektu
Tento projekt je organizovaný formou postupných úloh. Každá úloha je definovaná v samostatnom Markdown súbore a
predstavuje jeden logický krok vo vývoji aplikácie.

- [Úloha č. 1: Základné Stavebné Kamene (Dátové Objekty a Kontrakt)](uloha_01.md)

## Úloha č. 1: Základné Stavebné Kamene (Dátové Objekty a Kontrakt)

**Cieľ:**
- Vytvoriť základné dátové štruktúry a hlavné rozhranie pre náš bankový systém.
- V tejto fáze sa nebudeme zaoberať logikou (poplatky, limity), ale len definíciou "čo" sú naše dáta a "čo" má vedieť robiť každý účet.

**Požiadavky:**
1. Dátové Objekty (ideálne ako `record`):
    - `Customer`: Trieda reprezentujúca klienta. Zatiaľ stačí, ak bude mať atribút `name` (String).
    - `LegalGuardian`: Trieda reprezentujúca zákonného zástupcu. Mala by obsahovať `firstName` a `lastName` (String).
    - `AccountDetail`: Vytvorte rozhranie s týmto názvom. Bude slúžiť ako spoločný typ pre všetky dátové detaily účtov.
    - `KidsAccountDetail`: Konkrétna implementácia `AccountDetail`, ktorá bude obsahovať referenciu na `LegalGuardian`.
    - `BusinessAccountDetail`: Konkrétna implementácia `AccountDetail`, ktorá bude obsahovať `companyName` (String).
    - `StandardAccountDetail`: Konkrétna implementácia `AccountDetail`, ktorá nebude obsahovať žiadne dáta navyše (bude prázdna).
2. Klasifikácia Účtov (Enum):
    - `AccountProfile`: Vytvorte `enum`, ktorý bude presne zodpovedať hierarchii, o ktorej sme sa bavili. Mal by obsahovať hodnoty:
    - `PERSONAL_STANDARD`
    - `PERSONAL_STUDENT`
    - `PERSONAL_CHILD`
    - `BUSINESS_FREELANCER`
    - `BUSINESS_STANDARD`
    - `BUSINESS_PREMIUM`
4. Hlavný Kontrakt (Interface):
   - `BankAccount`: Vytvorte rozhranie, ktoré bude definovať spoločné operácie pre všetky typy účtov. Malo by obsahovať hlavičky (signatúry) nasledujúcich metód:
   - `getAccountName()`: Vráti `String`.
   - `getBalance()`: Vráti `BigDecimal`.
   - `getOwner()`: Vráti `Customer`.
   - `deposit(BigDecimal amount)`
   - `withdraw(BigDecimal amount)`
     
**Inštrukcie:**
- Sústreďte sa len na správnu definíciu tried, record-ov, enum-u a rozhraní.
- Nemusíte zatiaľ vytvárať žiadnu triedu, ktorá by implementovala BankAccount.
- Používajte java.math.BigDecimal pre všetky finančné sumy.
**Výzva na zamyslenie:**
- Prečo je v tomto prípade sealed rozhranie Account dobrý nápad, ale PersonalAccount je lepšie ako non-sealed?
- Ako zabezpečíte, aby bola trieda StudentPersonalAccount nemenná (immutable)?

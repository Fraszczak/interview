# Zadanie 2: Serwis kredytowy

## Kontekst

Rozszerz aplikację o serwis, który będzie zawierał logikę biznesową obliczania raty kredytu. Serwis powinien być używany przez komponent z zadania 1.

## Wymagania

### Serwis `CreditService`

**Metoda:**
calculatePayment(credit: CreditRequest): CreditResponse

**Wymagania:**

- Użyj proper TypeScript types/interfaces:
  - `CreditRequest` - interface dla danych wejściowych
  - `CreditResponse` - interface dla wyniku obliczeń
- Serwis powinien być injectable i dostępny w całej aplikacji.
- Zaimplementuj użycie serwisu w komponencie z zadania 1

**Struktura danych:**

`CreditRequest` powinien zawierać:

- `amount: number` - kwota kredytu
- `period: number` - okres spłaty w miesiącach
- `type: 'personal' | 'mortgage' | 'car'` - typ kredytu

`CreditResponse` powinien zawierać:

- `monthlyPayment: number` - miesięczna rata
- `totalAmount: number` - całkowita kwota do spłaty (opcjonalnie)
- `interest: number` - całkowite odsetki (opcjonalnie)

**Logika obliczania:**

- Możesz użyć prostego wzoru: `rata = kwota / okres`

## Wskazówki techniczne

- Zdefiniuj interfaces w tym samym pliku lub osobnym pliku types
- Wstrzyknij serwis do komponentu przez constructor (Dependency Injection)
- Zastąp prostą logikę obliczania w komponencie wywołaniem metody serwisu

## Uwagi

- Serwis powinien być niezależny od komponentu (może być używany w wielu miejscach)
- Logika obliczania powinna być w serwisie, nie w komponencie

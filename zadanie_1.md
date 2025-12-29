# Zadanie 1: Komponent formularza kredytowego

## Kontekst

Stwórz komponent formularza, który pozwoli użytkownikowi wprowadzić dane kredytu i obliczyć miesięczną ratę.

## Wymagania

### Komponent `CreditFormComponent`

**Pola formularza:**

- **Kwota kredytu** (number) - input numeryczny
- **Okres spłaty** (number) - input numeryczny (w miesiącach)
- **Typ kredytu** (dropdown) - wybór z opcji:
  - `'personal'` - Kredyt osobisty
  - `'mortgage'` - Kredyt hipoteczny
  - `'car'` - Kredyt samochodowy

**Funkcjonalność:**

- Formularz z polami input i select
- Przycisk "Oblicz ratę"
- Po kliknięciu przycisku wyświetl obliczoną miesięczną ratę
- Prosty wzór: `rata = kwota / okres`

**Walidacja:**

- Kwota kredytu: wymagana, minimum 1000 PLN, maksimum 500000 PLN
- Okres spłaty: wymagany, minimum 6 miesięcy, maksimum 360 miesięcy
- Typ kredytu: wymagany
- Wyświetlaj komunikaty błędów walidacji przy każdym polu
- Przycisk "Oblicz ratę" powinien być zablokowany gdy formularz jest nieprawidłowy

**Wyświetlanie wyniku:**

- Pokaż obliczoną miesięczną ratę po kliknięciu przycisku
- Formatuj liczbę (np. 2 miejsca po przecinku)

## Wskazówki techniczne

- Użyj **standalone component** (Angular 21)
- Możesz wybrać między **Reactive Forms** lub **Template Driven Forms**
- Użyj proper TypeScript types/interfaces dla danych formularza
- Komponent powinien być gotowy do użycia w aplikacji

## Przykład użycia

Po wprowadzeniu danych:

- Kwota: 100000 PLN
- Okres: 60 miesięcy
- Typ: Osobisty

Po kliknięciu "Oblicz ratę" powinna wyświetlić się rata: **1666.67 PLN**

## Uwagi

- Walidacja jest wymagana - użyj wbudowanych validators Angular (min, max, required)
- Skup się na działającym formularzu z walidacją i wyświetlaniu wyniku
- Możesz użyć prostego stylowania lub pozostawić domyślne

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

- Nie musisz implementować walidacji
- Skup się na działającym formularzu i wyświetlaniu wyniku
- Możesz użyć prostego stylowania lub pozostawić domyślne

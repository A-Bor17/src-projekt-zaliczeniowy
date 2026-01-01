# Inspiracje

## Opis
### Neologizmy i słowa z języka codziennego w języku angielskim

## Interface
### Okna dialogowe

## Listy
- *year*
- *country*

## Język
- `C++`

## Baza danych
### SQL lub Windows Server Manager

## Kategoria
- the_word_of_the_year_UK
- the_word_of_the_year_Japan

## Funkcje
- *while*
- *void*
- *if*

## Lista źródeł pomysłu
- potrzeba

## Przykładowy fragment kodu (C++):
```cpp
cout << "Choose the country of origin of the term:\n";
cin >> countryInput;

if (countryInput == "UK")
{
    cout << "Choose the year from 2004 to 2025:\n";
    cin >> yearInput;

    if (wordData["UK"].count(yearInput))
    {
        cout << "\nThe word of the year " << yearInput << " is:\n";
        auto [word, definition] = wordData["UK"][yearInput];
        cout << word << " - " << definition << "\n";
    }
}



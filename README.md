# tuziemia.pl – plugin

**Wyszukiwarka i analityka działek na sprzedaż w Polsce** dla asystentów AI (Claude, ChatGPT/Codex i inni klienci MCP).

[tuziemia.pl](https://tuziemia.pl) to polski portal z działkami na sprzedaż, na którym każda oferta ma granice działki na mapie, identyfikator ewidencyjny i dane z rejestrów publicznych.

## Co potrafi

- **Wyszukiwanie działek** w dowolnej gminie, mieście, powiecie lub województwie.
  - Filtry: cena, powierzchnia, rodzaj (budowlana, rolna, leśna, inwestycyjna, rekreacyjna).
  - Sortowanie: od najnowszych, najtańszych, największych.
- **Szczegóły działki:**
  - cena i powierzchnia;
  - przeznaczenie w planie ogólnym gminy;
  - użytki z ewidencji gruntów;
  - ostrzeżenia o pobliskich źródłach uciążliwości oraz planowanych i budowanych drogach i liniach kolejowych.
- **Ceny gruntów w okolicy:** mediany cen ofertowych z tuziemia.pl oraz rzeczywiste ceny transakcyjne z Rejestru Cen Nieruchomości z ostatnich 12 miesięcy.

Każdy wynik zawiera link do oferty na tuziemia.pl, gdzie są granice działki na mapie i kontakt do sprzedającego.

## Przykłady

- „Znajdź działki budowlane w gminie Kowala do 150 tys. zł”
- „Ile kosztuje metr działki w powiecie radomskim?”
- „Sprawdź działkę 142507_2.0012.2090/4: przeznaczenie w planie i co jest w okolicy”
- „Pokaż najtańsze działki rolne w województwie lubelskim”

## Zawartość

| Plik | Opis |
|---|---|
| `.mcp.json` | Zdalny serwer MCP `https://tuziemia.pl/mcp` (Streamable HTTP, bez logowania) |
| `skills/tuziemia/SKILL.md` | Wskazówki dla asystenta: kiedy i jak używać narzędzi |
| `.claude-plugin/plugin.json` | Manifest pluginu dla Claude |
| `.codex-plugin/plugin.json` | Manifest pluginu dla ChatGPT/Codex |

## Narzędzia (tylko odczyt)

| Narzędzie | Opis |
|---|---|
| `search_plots` | Lista aktualnych ofert (maks. 10) z linkami |
| `get_plot_details` | Szczegóły jednej aktywnej oferty |
| `area_land_prices` | Ceny ofertowe i transakcyjne w gminie, mieście lub powiecie |

## Prywatność

Plugin korzysta wyłącznie z publicznych danych tuziemia.pl i niczego nie zapisuje.

- **Czego nie zwraca:** imion, telefonów i adresów e-mail sprzedających ani numerów ksiąg wieczystych. Dane kontaktowe wpisane w opisy ofert są automatycznie usuwane.
- **Logowanie:** serwer nie wymaga logowania i nie przechowuje treści zapytań.
- **Więcej:** [polityka prywatności](https://tuziemia.pl/polityka-prywatnosci#asystenci-ai).

## Kontakt

kontakt@tuziemia.pl · [tuziemia.pl](https://tuziemia.pl)

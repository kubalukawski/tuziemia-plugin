# Zgłoszenie pluginu do katalogu Claude – wartości do formularza

## Plugin links

| Pole | Wartość |
|---|---|
| **Link to plugin** | `https://github.com/<twoje-konto>/tuziemia-plugin` (adres repozytorium z tym katalogiem) |
| **Path within repository** | puste – plugin jest w katalogu głównym repozytorium |
| **Plugin homepage** | `https://tuziemia.pl` |

## Plugin details

### Plugin name

tuziemia.pl

### Plugin description

Wyszukiwarka i analityka działek na sprzedaż w Polsce z portalu tuziemia.pl. Pozwala wyszukać aktualne oferty działek w dowolnej gminie, mieście, powiecie lub województwie, z filtrami ceny, powierzchni i rodzaju: budowlana, rolna, leśna, inwestycyjna, rekreacyjna. Dla wybranej działki pokazuje przeznaczenie w planie ogólnym gminy, użytki z ewidencji gruntów oraz ostrzeżenia o pobliskich uciążliwościach i planowanych drogach lub liniach kolejowych. Podaje też ceny gruntów w okolicy: mediany cen ofertowych i rzeczywiste ceny transakcyjne z Rejestru Cen Nieruchomości z ostatnich 12 miesięcy. Każdy wynik zawiera link do oferty z granicami działki na mapie. Plugin korzysta tylko z publicznych danych, działa w trybie tylko do odczytu i nie udostępnia danych osobowych sprzedających.

### Example use cases

Example 1: „Znajdź działki budowlane w gminie Kowala do 150 tys. zł”. Plugin zwraca listę aktualnych ofert z ceną, powierzchnią, ceną za m² i linkiem do każdej oferty.

Example 2: „Ile kosztuje metr działki w powiecie radomskim?”. Plugin podaje medianę cen ofertowych oraz medianę cen transakcyjnych z Rejestru Cen Nieruchomości z ostatnich 12 miesięcy.

Example 3: „Sprawdź działkę 142507_2.0012.2090/4: przeznaczenie w planie i co jest w okolicy”. Plugin pokazuje strefę z planu ogólnego gminy, użytki z ewidencji oraz ostrzeżenia, np. planowaną drogę ekspresową S12 ok. 350 m od działki.

Example 4: „Pokaż najtańsze działki rolne w województwie lubelskim”. Plugin zwraca oferty posortowane od najtańszych, z pominięciem ofert bez podanej ceny.

## Przed wysłaniem

1. Utwórz publiczne repozytorium na GitHubie (np. `tuziemia-plugin`) i wypchnij do niego ten katalog.
2. W `.claude-plugin/plugin.json` i `.codex-plugin/plugin.json` podmień pole `repository` (teraz `https://github.com/tuziemia/tuziemia-plugin`) na faktyczny adres repozytorium.
3. Ten plik zawiera tylko teksty do formularza. Nie musi trafić do repozytorium: usuń go albo dopisz do `.gitignore` przed pierwszym commitem.

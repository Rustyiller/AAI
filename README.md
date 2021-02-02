# AAI Project

Projekt wykonany na zajęcia AAI. Celem projektu jest stworzenie sieci, która będzie w stanie rozpoznawać typy ubrania takie jak spodnie, sukienka czy koszula oraz kolory owych ubrań.

Przykłady ubrań wykorzystanych w projekcie:
* Czarne spodnie,
* Niebieska sukienka,
* Niebieskie spodnie,
* Niebieska koszula,
* Czerwona sukienka,
* Czerwona koszula

## Wczytanie potrzebnych bibliotek
Wszystkie wykorzystanie biblioteki znajdują się w pliku requirements.txt

pip install -r requirements.txt

## Przykład komendy do utworzenia wytrenowania modelu

python train.py -d dataset -e 50 -m model_50e

d - ścieżka do folderu ze zdjęciami treningowymi
e - ilość epok
m - nazwa modelu

Po wytrenowaniu modelu powinien w głównym katalogu pojawić się wykres pokazujący accuracy i loss podczas trenowania modelu.

## Przykład komendy testowania wytrenowanego modelu

python classify.py -m model_50e -t test

t - ścieżka do folderu ze zdjęciami testowymi

## Model sieci SmallerVGGNet
Model sieci bazowany jest na poniższym diagramie. Model ten w oryginalnym projekcie był wykorzystywany do rozpoznawania Pokemonów.
Link do projektu: https://github.com/sksoumik/machine-learning-projects/blob/master/pokemon_classification_cnn/cnn-keras/pyimagesearch/smallervggnet.py

![https://pyimagesearch.com/wp-content/uploads/2018/04/smallervggnet_model.png](https://pyimagesearch.com/wp-content/uploads/2018/04/smallervggnet_model.png)

# Predykcja sprzedaży - prototyp (sieci neuronowe)

Cel: przygotowanie podejścia do budowy modelu predyckji sprzedaży tak by odpowidzieć na pytania a. jak zamodelować dane b. jak skonstruować sieć, która wykona predykcję dla wielu produktów jednocześnie (na wejściu wiele serii i na wyjściu wiele serii).

<ins>**Zrobione:**</ins>
- opracowana koncepcja przygotowania danych w różnych konfiguracjach sieci (z algorytmem ramkowania danych - windowing i subwindowing)
- przykładowe architektury (do przyszłej rozbudowy) - Encoder-Decoder (LSTM), Vector (CNN, Vanila LSTM, CNN-LSTM)
- testy predykcji
- dwa przykładowe callbacki 

<ins>**Do zrobienia:**</ins>
- przygotowanie realnych danych sprzedażowych
- przygotowanie zbioru trening, walidacja, test (tutaj zrobiłem tylko trening) 
- konfiguracja sieci - wybór architektury (sugerowane CNN-LSTM lub Conv2LSTM - nie opracowano tutaj ale podobne do CNN-LSTM) 
- optymalizacja hiperparametrów
- optymalizacja doboru długości okna próbkującego i pod okna (w konfiguracji CNN-LSTM)


<ins>**Do rozważenia:**</ins>
- architektura modelu - dla każdego produktu oddzielny model, dla wszystkich produktów model, dla grup produktów modele
- podejście do modelowania danych -  A. produkty (x), produkty (y), B. cechy środowiska (x), produkty (y)

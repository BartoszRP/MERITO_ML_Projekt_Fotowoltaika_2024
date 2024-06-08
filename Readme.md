# Projekt Fotowoltaika 2024

Projekt Fotowoltaika 2024 ma na celu analizę i przewidywanie wyników z instalacji fotowoltaicznych. Projekt wykorzystuje dane, modele uczenia maszynowego oraz skrypty do wizualizacji danych w celu zrozumienia i optymalizacji efektywności paneli słonecznych.

## Struktura katalogów

1. **Notebooks**: Zawiera Jupyter notebooks z analizami danych i przetwarzaniem:
    - `00-okreslenie_celu_i_wymagan_projektu.ipynb` - Określenie celu i wymagań projektu.
    - `01-pobieranie_i_przetwarzanie_danych.ipynb` - Skrypty do pobierania i pierwszego przetwarzania danych.
    - `02-inicjalizacja_bazy_danych.ipynb` - Skrypt do inicjalizacji bazy danych.
    - `03-analiza_danych.ipynb` - Analiza zbieranych danych.
    - `04-wizualizacja_dashboard_danych.ipynb` - Wizualizacja danych na dashboardzie.

2. **Data**:
    - **ML_models**: Modele uczenia maszynowego.
    - **processed**: Przetworzone dane.
    - **raw**: Surowe dane.

3. **Scripts**:
    - `starter_brak_Data.ipynb` - Skrypt uruchamiany gdy brak danych w `Data/processed`.
    - `starter_Data_istnieje_Wizualizacja.ipynb` - Skrypt uruchamiany gdy dane są już dostępne w `Data/processed`.

4. **ML_Models**:
    - `05-pobieranie_i_przygotowanie_danych.ipynb`
    - `06-Wizualizacja_z_predykcja.ipynb`

5. **Baza_Danych**:
    - `projekt_fotowoltaika_2024.db` - Baza danych projektu.

6. **Docs**: Dokumentacja projektu.

7. **Requirements**:
    - `requirements.txt` - Zależności projektu.

## Uruchomienie projektu

Aby uruchomić projekt, potrzebne są następujące kroki:

1. **Instalacja zależności**:
    ```
    pip install -r Requirements/requirements.txt
    ```

2. **Uruchomienie odpowiedniego skryptu w zależności od dostępności danych**:
    - Jeśli dane są już przetworzone:
        ```
        jupyter notebook Scripts/starter_Data_istnieje_Wizualizacja.ipynb
        ```
    - Jeśli dane nie są dostępne i trzeba je przetworzyć:
        ```
        jupyter notebook Scripts/starter_brak_Data.ipynb
        ```

## Wymagania

- Python 3.9.1
- Pozostałe zależności są wymienione w pliku `Requirements/requirements.txt`.

## Licencja

Projekt jest objęty licencją X (specyfikuj rodzaj licencji, jeśli to konieczne).

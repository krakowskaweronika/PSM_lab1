# Laboratorium 1
Autor: Weronika Krakowska

# Zadanie 3
<img width="1423" height="879" alt="zad3" src="https://github.com/user-attachments/assets/fc9046bd-c76d-4ce8-9ba2-916a78b7dbb9" />

---

# Zadanie 4
<img width="362" height="167" alt="zad4" src="https://github.com/user-attachments/assets/c8b86a53-ca62-4562-8708-5ee7e8c269b9" />

---

# Zadanie 5
<img width="489" height="930" alt="zad5" src="https://github.com/user-attachments/assets/3bcbf8ca-e8c1-4b46-bafb-1ed416c1c127" />

---

# Zadanie 6
<img width="1506" height="949" alt="zad6" src="https://github.com/user-attachments/assets/b7633f88-11e3-457e-b5d4-31af0552faa6" />

---

# Zadanie 7
<img width="1840" height="893" alt="azd7" src="https://github.com/user-attachments/assets/35a0b606-9a5f-4c4c-a496-4ad9c47ccd43" />

---

# Sprawozdanie – Zadanie 8: Porównanie obu podejść

## 1. Analiza wariantów (liczba plików i czas kompilacji)
* **Jetpack Compose (Kotlin):** Wymagało edycji **2 plików** (`MainActivity.kt` oraz `strings.xml`). Czas kompilacji jest krótki, a cała logika interfejsu zamyka się w jednym pliku kodu.
* **Views (Java + XML):** Wymagało edycji **4 plików** (`build.gradle.kts`, plik układu XML, `strings.xml`, `MainActivity.java`). Czas kompilacji jest zauważalnie dłuższy przez konieczność przetwarzania plików XML oraz generowania klas View Binding.

## 2. Tabela obserwacji

| Zagadnienie | Jetpack Compose (Kotlin) | Views (Java + XML) |
| :--- | :--- | :--- |
| **Opis interfejsu** | kod Kotlina, funkcje @Composable | plik XML + kod aktywności |
| **Liczba edytowanych plików** | 2 (`MainActivity.kt`, `strings.xml`) | 4 (`build.gradle.kts`, układ XML, `strings.xml`, `MainActivity.java`) |
| **Dostęp do kontrolek** | niepotrzebny – stan steruje widokiem | View Binding (dawniej `findViewById`) |
| **Ukrywanie elementu** | element nie powstaje (`if`) | atrybut `visibility: invisible / gone` |
| **Podgląd interfejsu** | `@Preview` w IDE | edytor układu (Design / Split) |
| **Reakcja na zmianę danych** | automatyczna rekompozycja | ręczna aktualizacja kontrolek |
| **Czas kompilacji** | krótki, szybki podgląd dzięki `@Preview` | dłuższy ze względu na narzut XML i View Binding |
| **Czytelność kodu** | wysoka, cała logika interfejsu w jednym pliku | średnia/niska, rozproszona pomiędzy pliki XML a Javę |

## 3. Podsumowanie
Podejście oparte na Jetpack Compose okazało się czytelniejsze i wygodniejsze, ponieważ eliminuje potrzebę rozpraszania kodu pomiędzy pliki układu XML a klasę aktywności, pozwalając na deklaratywne zarządzanie interfejsem w jednym miejscu.

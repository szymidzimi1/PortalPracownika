# System Zarządzania Czasem Pracy (Projekt Zaliczeniowy)

**Autorzy:** Szymon Nowacki, Hubert Mościcki  
**Technologie:** PHP, MySQL, HTML/CSS

Prosty portal webowy przeznaczony do ewidencji i zarządzania czasem pracy w firmie z podziałem na role użytkowników.

---

## Funkcjonalności ogólne
* **System użytkowników:**
  * Rejestracja konta (nowe konta domyślnie otrzymują uprawnienia inne niż `1` i oczekują na aktywację).
  * Logowanie warunkowe (dostęp po aktywacji konta przez Administratora).
  * Zmiana hasła po zalogowaniu.
* **Bezpieczeństwo i obsługa danych:**
  * Bezpieczne haszowanie haseł.
  * Walidacja danych wprowadzanych przez formularze.
  * Dodawanie informacji do bazy za pośrednictwem formularzy.

---

## Role i Uprawnienia

### 1. Pracownik (Uprawnienie: `1`)
* Wyświetlanie własnych dni i czasu pracy (**GODZINY PRACY**).
* Dodawanie komentarzy do swoich dni pracy.

### 2. Kierownik (Uprawnienie: `2`)
* Podgląd dni i czasu pracy wszystkich pracowników (**KARTY PRACY**).
* Wyświetlanie własnych dni i czasu pracy (**GODZINY PRACY**).
* Dodawanie czasu pracy dla siebie.
* Dodawanie czasu pracy dla innych pracowników.
* Komentowanie dni i czasu pracy wszystkich użytkowników.

### 3. Administrator (Uprawnienie: `3`)
* Wyświetlanie własnych dni i czasu pracy (**GODZINY PRACY**).
* Pełne zarządzanie użytkownikami (operacje **CRUD**: tworzenie, odczyt, aktualizacja, usuwanie oraz aktywacja kont).

---

## Dane testowe do logowania

| Rola / Użytkownik | Login | Hasło | Uwagi |
| :--- | :--- | :--- | :--- |
| **Administrator** | `Admin` | `Admin` | Pełny dostęp |
| **Administrator 2** | `Admin2` | `Admin2` | Konto administracyjne |
| **Kierownik** | `Kierownik` | `Kierownik` | Dostęp kierowniczy |
| **Pracownik 1** | `Pracownik1` | `Pracownik1` | *Konto nieaktywne (do testowania blokady)* |
| **Pracownik 2** | `Pracownik2` | `Pracownik2` | Konto aktywne |
| **Pracownik 3** | `Pracownik3` | `Pracownik3` | Konto aktywne |

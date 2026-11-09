Poniżej masz gotowy plik README.md do wrzucenia na GitHuba. Jest napisany w języku polskim, zawiera opis projektu, funkcje, wykaz komponentów, schemat podłączenia oraz instrukcję obsługi.

Pisanie

# 🧮 Kalkulator Arduino UNO

## 📌 Opis projektu

Projekt przedstawia prosty kalkulator zbudowany na platformie **Arduino UNO**. Urządzenie umożliwia wykonywanie podstawowych operacji matematycznych przy użyciu klawiatury membranowej 4x4 oraz wyświetlacza LCD 16x2 z interfejsem I2C.

Wyniki obliczeń są wyświetlane na ekranie LCD z dokładnością do dwóch miejsc po przecinku.

## ⚙️ Funkcjonalności

- Dodawanie dwóch liczb (+)
- Odejmowanie dwóch liczb (-)
- Mnożenie dwóch liczb (\*)
- Dzielenie dwóch liczb (/)
- Wyświetlanie wyniku na ekranie LCD
- Obsługa błędu dzielenia przez zero
- Możliwość wyczyszczenia wprowadzonych danych
- Ograniczenie długości wpisywanej liczby do 10 cyfr

## 🛠️ Wykorzystane komponenty

- Arduino UNO
- Wyświetlacz LCD 16x2 z modułem I2C
- Klawiatura membranowa 4x4
- Przewody połączeniowe
- Płytka stykowa (opcjonalnie)

## 🔌 Schemat podłączenia

### Wyświetlacz LCD I2C

| LCD I2C | Arduino UNO |
| --- | --- |
| VCC | 5V |
| GND | GND |
| SDA | A4 |
| SCL | A5 |

### Klawiatura 4x4

| Pin klawiatury | Pin Arduino UNO |
| --- | --- |
| R1 | 9 |
| R2 | 8 |
| R3 | 7 |
| R4 | 6 |
| C1 | 5 |
| C2 | 4 |
| C3 | 3 |
| C4 | 2 |

## 🎮 Instrukcja obsługi

Klawiatura została skonfigurowana w następujący sposób:

| Przycisk | Funkcja |
| --- | --- |
| 0–9 | Wprowadzanie liczb |
| A | Dodawanie (+) |
| B | Odejmowanie (-) |
| C | Mnożenie (\*) |
| D | Dzielenie (/) |
| # | Obliczenie wyniku |
| \* | Reset kalkulatora |

### Przykład działania

Aby wykonać działanie 15 + 5:

1. Wciśnij `1`.
2. Wciśnij `5`.
3. Wciśnij `A` (dodawanie).
4. Wciśnij `5`.
5. Wciśnij `#`, aby wyświetlić wynik.

Na wyświetlaczu pojawi się:

text

```text
Wynik:
20.00
```

## 📚 Wymagane biblioteki

Przed uruchomieniem programu należy zainstalować następujące biblioteki w Arduino IDE:

- `Wire.h` – obsługa komunikacji I2C.
- `Adafruit_LiquidCrystal.h` – obsługa wyświetlacza LCD.
- `Keypad.h` – obsługa klawiatury matrycowej.

## 🚀 Uruchomienie projektu

1. Podłącz wszystkie komponenty zgodnie z tabelami.
2. Otwórz Arduino IDE.
3. Zainstaluj wymagane biblioteki.
4. Otwórz plik z kodem `.ino`.
5. Wybierz płytkę Arduino UNO.
6. Wybierz odpowiedni port COM.
7. Wgraj program na mikrokontroler.
8. Po uruchomieniu korzystaj z kalkulatora za pomocą klawiatury.

## 🧠 Technologie

- C++
- Arduino IDE
- Platforma Arduino UNO
- Komunikacja I2C

## 👨‍💻 Autor

Projekt edukacyjny wykonany z wykorzystaniem platformy Arduino UNO.

## 📄 Licencja

Projekt udostępniony do celów edukacyjnych. Można go rozwijać, modyfikować i wykorzystywać do nauki programowania mikrokontrolerów.

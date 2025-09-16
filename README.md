# Digispark Support (ATtiny85, Rev3)

To repozytorium zawiera sterowniki USB oraz pliki **Boards Manager JSON** potrzebne do pracy z płytką **Digispark ATtiny85 (Rev 3)** w środowisku Arduino IDE.

## 📦 Zawartość
- `drivers/` – sterowniki Digistump USB (Windows, DPinst.exe).
- `package_digistump_index.json` – oryginalny plik Boards Manager.
- `package_digistump_index_arminjo.json` – utrzymywana wersja ArminJo (zalecana).

---

## 🔧 Instalacja sterowników (Windows)
1. Otwórz folder `drivers/`.
2. Uruchom `DPinst.exe` (lub `DPinst64.exe` na systemie 64-bitowym).
3. Zainstaluj sterowniki USB (libusb dla Digisparka).
4. Na Linux/Mac sterowniki zwykle nie są potrzebne.

---

## ⚙️ Instalacja w Arduino IDE

### 1. Dodanie URL w Arduino IDE
Otwórz: **File → Preferences → Additional Board Manager URLs** i dodaj:

- dla oryginalnej paczki:

- https://github.com/Bertos/digispark-support/blob/main/digispark-support/package_digistump_index.json

- dla paczki ArminJo

- https://github.com/Bertos/digispark-support/blob/main/digispark-support/package_digistump2_index.json

### 2. Instalacja pakietu
1. Wejdź w **Tools → Board → Boards Manager**.
2. Wyszukaj `Digistump AVR Boards`.
3. Kliknij **Install**.

### 3. Wybór płytki
- **Tools → Board → Digispark (Default - 16.5 MHz)** dla zwykłego Digispark Rev 3.

---

## 🚀 Programowanie Digisparka
1. Wybierz płytkę jak wyżej.
2. Kliknij **Upload** w Arduino IDE.
3. Gdy pojawi się komunikat *"Podłącz płytkę..."* – wtedy dopiero włóż Digisparka do USB.
4. Kod zostanie wgrany przez USB (bez portu COM).

---

## ℹ️ Uwagi
- Arduino IDE **1.8.19** jest bardziej kompatybilne niż 2.x.
- ATtiny85 ma ograniczoną pamięć (8 KB Flash, 512 B RAM), nie wszystkie biblioteki Arduino się zmieszczą.
- Przydatne biblioteki:
- `TinyWireM` – I²C,
- `DigiUSB` – komunikacja USB,
- `Adafruit_NeoPixel` – sterowanie WS2812,
- `SoftwareSerial` – dodatkowy UART.

---

✍️ Repozytorium przygotowane, aby zawsze mieć **lokalną kopię sterowników i definicji płytek**, niezależną od zewnętrznych serwerów.

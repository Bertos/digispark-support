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

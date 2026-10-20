# Inferno – płonące pola danych dla Hammerhead Karoo 2

Rozszerzenie (Karoo Extension) dodające animowane pola danych w stylu **Inferno**:
płonąca wskazówka prędkości, płonący pasek mocy, tętno w formie EKG i kadencja.

- od **30 km/h** płonie wskazówka i tarcza prędkości,
- od **50 km/h** ogień obejmuje krawędzie pola,
- od **300 W** płonie pasek mocy.

Pola: Ekran Inferno, Prędkość, Moc, Tętno, Kadencja (Inferno).

## Pobierz

**[⬇ Pobierz najnowszą wersję (APK)](https://github.com/Handloteka/karoo-inferno/releases/latest/download/inferno.apk)**

Wszystkie wersje: [Releases](https://github.com/Handloteka/karoo-inferno/releases)

## Instalacja

### Bez kabla – aplikacja Hammerhead Companion (jeśli Twój licznik to obsługuje)
1. Na telefonie skopiuj link „Pobierz najnowszą wersję” powyżej.
2. Udostępnij go do aplikacji **Hammerhead Companion** (Udostępnij → Hammerhead).
3. Potwierdź instalację na liczniku.

### Przez kabel USB (ADB) – działa zawsze
1. Na Karoo: **Ustawienia → Informacje** → stuknij kilka razy w **numer kompilacji**, aż włączy się tryb programisty. Następnie w **Opcjach programisty** włącz **Debugowanie USB**.
2. Na komputerze pobierz [SDK Platform-Tools](https://developer.android.com/tools/releases/platform-tools) i rozpakuj. Do tego folderu skopiuj `inferno.apk`.
3. Podłącz Karoo kablem, otwórz w tym folderze wiersz poleceń i wpisz:
   ```
   adb devices
   adb install -r inferno.apk
   ```
   Na liczniku zatwierdź „Zezwolić na debugowanie USB?”. Komunikat `Success` = gotowe.
4. Dodaj pola Inferno do ekranu jazdy w ustawieniach profilu na Karoo.

Odinstalowanie: `adb uninstall pl.handloteka.inferno`

## Uwagi
- Animacje mogą zwiększyć zużycie baterii.
- Aplikacja jest udostępniana bezpłatnie, „tak jak jest”, bez gwarancji. Nie jest powiązana z Hammerhead.

---

## English

Animated "Inferno" data fields for the **Hammerhead Karoo 2**: flaming speed needle (from 30 km/h, edges from 50 km/h), flaming power bar (from 300 W), ECG heart rate and cadence.

**[Download latest APK](https://github.com/Handloteka/karoo-inferno/releases/latest/download/inferno.apk)** · install via Hammerhead Companion app (share the link) or `adb install -r inferno.apk`.

Provided free, as is, without warranty. Not affiliated with Hammerhead.

© Handloteka · [handloteka.net](https://handloteka.net)

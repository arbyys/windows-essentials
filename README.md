# Windows essentials

Užitečné kroky po instalaci systému Windows

___

#### Instalace, aktivace systému, základní nastavení:
- Zálohovat nastavení starého systému na Microsoft účet
- Vytvořit instalační médium
  - [pro Windows 10](https://www.microsoft.com/cs-cz/software-download/windows10)
  - [pro Windows 11](https://www.microsoft.com/cs-cz/software-download/windows11)
- Nainstalovat z flashky
- Při instalaci zvolit "nemám aktivační klíč"
- Aktivace Windowsu
  - [aktivační software](src/winactivate)
  - spustit soubor `winactivate.cmd` s admin právy
- V nastavení:
  - `Systém -> Multitasking -> Zatřepání okna záhlaví` - vypnout
  - `Systém -> Napájení -> Obrazovka -> Režim spánku` - nastavit podle potřeby
  - `Přizpůsobení -> Hlavní panel` - nastavit dle potřeby + vypnout zbytečnosti v hlavním panelu
- Případně aktualizovat drivery
___

#### Zásahy do registrů:
- Vrácení Windows Photo Viewer jako defaultní aplikace pro prohlížení obrázků
  - [složka se souborem pro editaci registrů](src/photoviewer)
  - spustit soubor `windows_photo_viewer.reg`
- **[Win11]** Vrácení starého kontextového menu při kliknutí pravým tlačítkem
  - [složka se souborem pro editaci registrů](src/contextmenu)
  - spustit soubor `context_menu.reg`
- Zrušení Bing vyhledávání ve Windows nabídce v případě žádné shody
  - [složka se souborem pro editaci registrů](src/disablebing)
  - spustit soubor `disable_bing_search.reg`
  - ve správci úloh restartovat proces `explorer.exe`
- Zobrazení přípon souborů + zobrazení skrytých souborů
  - [složka se souborem pro editaci registrů](src/filesettings)
  - spustit soubor `file_settings.reg`
___

#### Programy přepisující defaultní windows funkce:

- EarTrumpet (náhrada za směšovač hlasitost)
  - v PowerShellu spustit příkaz `winget install -e --id File-New-Project.EarTrumpet`
- **[Win11]** ElevenClock (náhrada za defaultní hodiny - na Win11 nejsou hodiny na všech monitorech)
  - v PowerShellu spustit příkaz `winget install -e --id SomePythonThings.ElevenClock`
- ShareX (náhrada za výstřižky)
  - v PowerShellu spustit příkaz `winget install -e --id ShareX.ShareX`

___

#### Další užitečné funkce

- **[Win10]** Debloater
  - [soubor Debloater GUI](src/debloater)
  - spustit soubor `windows10debloater.ps1` v PowerShellu

# Użycie templatek w Obsidian

## Menu
- [Start](#start)
- [Rozpoczęcie pracy](#rozpoczęcie-pracy)
- [Instalacja wtyczki](#instalacja-wtyczki)
- [Użycie templatek](#użycie-templatek)


### Start

Sprawdzenie czy Obsidian jest zainstalowany (Kali VM, jako App Image).
   
  `find ~ -type f -name "Obsidian*.AppImage" 2>/dev/null`
  
Jeżeli terminal zwróci ścieżkę - zainstalowany, jeżeli nie to instalacja.

   `sudo apt install obsidian`

### Rozpoczęcie pracy

1. Stworzenie sejfu

<img width="300" height="300" alt="1" src="https://github.com/user-attachments/assets/91dbf094-0756-427a-89b1-3b1629c14719" />

2. Skopiowanie do sejfu folderu Templates

   a) git - komenda w terminalu w dowolnym folderze
   
   `git clone https://github.com/tnisoCode/obsidianTemplates.git`   
   `cd obsidianTemplates`   
   `cp -r Templates ~/lokalizacja_twojego_sejfu`    

   b) lub ściagnij pliki z foldery Templates do twojego sefu i folderu gdzie trzymane będą templatki (stwórz).

### Instalacja wtyczki

   a) kliknij w ikonę trybika (dolna część okna głównego w Obsidianie) żeby wejść do ustawień ogólnych  
   b) kliknij "Community Plugins" -> wybierz "Turn on community plugins" -> kliknij "Browse" w sekcji "Community Plugins"  
   c) w okienku wyszukiwania wpisz "Templater" i kliknij okienko wtyczki po wyszukaniu  

   <img width="500" height="500" alt="2" src="https://github.com/user-attachments/assets/ff5db682-0268-45fa-927f-3352ed44f159" />

   d) kliknij "Install", a po instalacji "Enable", wyłącz okienko  
   e) plugin powinien byc juz widoczny w zaintalowanych "Community Plugins" - kliknij ikonę trybika na zakładce Templater  

   <img width="500" height="500" alt="3" src="https://github.com/user-attachments/assets/4c666e87-d1fc-4269-8a47-983cbca2ef5b" />
      
      
   f) ustaw folder dla templatek na ten do którego skopiiowałeś templatki w twoim sejfie -> "Template folder location"   
   g) wyłącz pokazywanie templatek na grafie - kliknij ikonę trybika ustawień głównych Obsidian (jak w punkcie 4.a) -> "Files and links" -> w sekcji Advanced kliknij "Excluded files" i wskaż folder templatek do wykluczenia i kliknij "Save"

### Użycie Templatek

Po uruchomieniu Obsidiana i wybraniu sejfu na którym chcesz pracować, pracy wklik w zakładce eksploratora plików i wybór templatek z wtyczki Templatera do stworzenia nowej notatki
   
<img width="500" height="500" alt="4" src="https://github.com/user-attachments/assets/0a0d7ec9-d12d-4a87-ab8e-35c74ee86125" />

   

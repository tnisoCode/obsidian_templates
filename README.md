# Użycie templatek w Obsidian

Cel: co daje zastosowanie wtyczki Templater ?

Umożliwia dynamiczne wstawianie dat, automatyczne nazywanie plików, używanie skryptów JavaScript oraz zaawansowaną manipulację danymi wewnątrz notatek.

## Menu
- [Start](#start)
- [Rozpoczęcie pracy](#rozpoczęcie-pracy)
- [Instalacja wtyczki](#instalacja-wtyczki)
- [Użycie templatek](#użycie-templatek)


### Start

Sprawdzenie czy Obsidian jest zainstalowany (Kali VM, jako App Image).
   
  `find ~ -type f -name "Obsidian*.AppImage" 2>/dev/null`
  
Jeżeli terminal zwróci ścieżkę - Obsidian jest zainstalowany, jeżeli jej nie będzie - to instalacja.

   `sudo apt install obsidian`

### Rozpoczęcie pracy

1. Stworzenie sejfu

   <img width="500" height="500" alt="1" src="https://github.com/user-attachments/assets/3c5afc39-f063-4afa-a215-945ed50a13a2" />   	


2. Skopiowanie do utworzonego sejfu folderu Templates

   a) git - komenda w terminalu w dowolnym folderze
   
   `git clone https://github.com/tnisoCode/obsidian_templates.git`   
   `cd obsidian_templates`   
   `cp -r Templates ~/lokalizacja_twojego_sejfu`    

   b) lub ściagnij pliki z folderu Templates (to repo) do twojego sefu (folderu gdzie trzymane będą templatki).

### Instalacja wtyczki

   a) kliknij w ikonę trybika (dolna część okna głównego w Obsidianie) żeby wejść do ustawień ogólnych  
   b) kliknij "Community Plugins" -> wybierz "Turn on community plugins" -> kliknij "Browse" w sekcji "Community Plugins"  
   c) w okienku wyszukiwania wpisz "Templater" i kliknij okienko wtyczki po wyszukaniu   

   <img width="500" height="500" alt="2" src="https://github.com/user-attachments/assets/6795f60e-ad02-4e0a-9aa7-134df5a842ca" />   	


   d) kliknij "Install", a po instalacji "Enable", wyłącz okienko  
   e) plugin powinien byc juz widoczny w zaintalowanych "Community Plugins" - kliknij ikonę trybika na zakładce Templater  

   <img width="500" height="500" alt="3" src="https://github.com/user-attachments/assets/41e9d3a1-b5c2-431f-998b-8401b6bcb400" />      	

      
   f) ustaw folder dla templatek na ten do którego skopiiowałeś templatki w twoim sejfie -> "Template folder location"   
   g) wyłącz pokazywanie templatek na grafie - kliknij ikonę trybika ustawień głównych Obsidian (jak w punkcie 4.a) -> "Files and links" -> w sekcji Advanced kliknij "Excluded files" i wskaż folder templatek do wykluczenia i kliknij "Save"

### Użycie Templatek

Po uruchomieniu Obsidiana i wybraniu sejfu na którym chcesz pracować, pracy wklik w zakładce eksploratora plików i wybór templatek z wtyczki Templatera do stworzenia nowej notatki
   
   <img width="500" height="500" alt="4" src="https://github.com/user-attachments/assets/d3d4a319-31aa-48a5-8a80-66d897cc85bb" />   


   

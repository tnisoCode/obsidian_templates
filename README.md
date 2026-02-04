# Użycie Obsidiana

*Czym jest Obsidian ?*

Obsidian to aplikacja do tworzenia notatek i zarządzania osobistą bazą wiedzy, działająca na lokalnych plikach tekstowych w formacie Markdown.	 
Umożliwia także tworzenie grafów powiązań.

Dokumentacja Obsidiana online: https://help.obsidian.md/



## Menu
- [Start](#start)
- [Rozpoczęcie pracy](#rozpoczęcie-pracy)
- [Instalacja wtyczek](#instalacja-wtyczek)
- [Użycie templatek](#użycie-templatek)
- [Podgląd i pisanie notatki](#podgląd-i-pisanie-notatki)
- [Tagi](#tagi)
- [Zapis notatki do pliku](#zapis-notatki-do-pliku)
- [Graf powiązań](#graf-powiązań)


### Start

1. Sprawdzenie czy Obsidian jest zainstalowany (Kali VM, jako App Image).
   
  `find ~ -type f -name "Obsidian*.AppImage" 2>/dev/null`
  
Jeżeli terminal zwróci ścieżkę - Obsidian jest zainstalowany, jeżeli jej nie będzie - to instalacja.

   `sudo apt install obsidian`	
   

2. Jeżeli w systemie nie ma polskiej klawiatury - należy ją ustawić.
   
Klikamy w symbol Kali(1), a następnie w ustawienia(2).	

<img width="300" height="300" alt="1a" src="https://github.com/user-attachments/assets/70340fa5-b3b2-47de-a1aa-46957b3e0130" />		     

Wybieramy keyboard i klikamy zakładkę Layout.     
Na zakładce Layout odznaczmy przełącznik Use system defaults (1), dodajemy pożądany język(2) (PL legacy(3)), usuwamy pozostałe języki(4) i zamykamy okienko(5).	

<img width="300" height="300" alt="4a" src="https://github.com/user-attachments/assets/6d607cb3-afaa-4b29-98d0-6116c82849f8" />



### Rozpoczęcie pracy

1. Stworzenie sejfu

   <img width="600" height="400" alt="1" src="https://github.com/user-attachments/assets/3c5afc39-f063-4afa-a215-945ed50a13a2" />   	


2. Skopiowanie do utworzonego sejfu folderu Templates

   a) ściagnij pliki z folderu Templates (to repo) do twojego sejfu (folder gdzie trzymane będą templatki - np. Templates)
   	
   b) lub użyj gita - komenda w terminalu w dowolnym folderze
   
   `git clone https://github.com/tnisoCode/obsidian_templates.git`   
   `cd obsidian_templates`   
   `cp -r Templates ~/lokalizacja_twojego_sejfu/Templates`

### Instalacja wtyczek

1. *Templater* - umożliwia dynamiczne wstawianie dat, automatyczne nazywanie plików, używanie skryptów JavaScript oraz zaawansowaną manipulację danymi wewnątrz notatek.     

   a) kliknij w ikonę trybika (dolna część okna głównego w Obsidianie) żeby wejść do ustawień ogólnych

<img width="600" height="400" alt="3aa" src="https://github.com/user-attachments/assets/bfd59e99-032e-48d4-ae7a-ff7a3e4db36a" />

	
   b) kliknij "Community Plugins" -> wybierz "Turn on community plugins" -> kliknij "Browse" w sekcji "Community Plugins"  
	
   c) w okienku wyszukiwania wpisz "Templater" i kliknij okienko wtyczki po wyszukaniu   

   <img width="600" height="400" alt="2" src="https://github.com/user-attachments/assets/6795f60e-ad02-4e0a-9aa7-134df5a842ca" />   	


   d) kliknij "Install", a po instalacji "Enable", wyłącz okienko  
	
   e) plugin powinien byc juz widoczny w zaintalowanych "Community Plugins" - kliknij ikonę trybika na zakładce Templater  
	
<img width="600" height="400" alt="3b" src="https://github.com/user-attachments/assets/3f0c664a-1598-43f7-bbb1-3b023c81cf40" />     
      
   f) ustaw folder dla templatek na ten do którego skopiiowałeś templatki w twoim sejfie -> "Template folder location"   
	
   g) wyłącz pokazywanie templatek na grafie - kliknij ikonę trybika ustawień głównych Obsidian -> "Files and links" -> w sekcji Advanced kliknij "Excluded files" i wskaż folder templatek do wykluczenia i kliknij "Save"
   


3. *Pandoc* - umożliwia zaawansowany eksport notatek Markdown do wielu formatów, takich jak DOCX, PDF, EPUB, LaTeX czy HTML.     

Kroki przechodzimy tak jak poprzednio przy instalacji Templatera. Wyszukujemy w pluginach po słowie Pandoc.

*UWAGA*

Po instalcji Pandoc, ścieżka może nie być wykrywana przez Obsidian.

`which pandoc`     

Powinniśmy otrzymać np. 

`/usr/bin/pandoc`     

Jeżeli jej nie dostajemy lub wyskakuje błąd - instalujemy Pandoc globalnie w systemie. 

`sudo apt update && sudo apt install pandoc`

Ponownie ściągamy ścieżkę.

`which pandoc`

Kopiujemy i wklejamy ją w ustawieniach wtyczki (1 i 2).

<img width="500" height="500" alt="9" src="https://github.com/user-attachments/assets/fc785088-ed0b-41b3-9e79-08791856fe6a" />     
<img width="500" height="500" alt="10" src="https://github.com/user-attachments/assets/aa4dfecd-2047-4929-b3da-2d4f7a97bfbc" />


### Użycie Templatek

Po uruchomieniu Obsidiana i wybraniu sejfu na którym chcesz pracować, pracy wklik w zakładce eksploratora plików i wybór templatek z wtyczki Templatera do stworzenia nowej notatki.     

*Ćwiczenie*: Dodaj nową notatkę z szblonu Person.	
   
   <img width="500" height="500" alt="4" src="https://github.com/user-attachments/assets/d3d4a319-31aa-48a5-8a80-66d897cc85bb" />   

### Podgląd i pisanie notatki

W okienku Obsidiana możemy przełączać pomiędzy edycją notatki(1) a podglądem(2) klikając w znaczek w dolnym prawym rogu (długopis, książka, kod - zależenie od załączonego trybu).     
W trybie podglądu niewidoczne będą znaczniki kodu oraz nie będziemy mogli edytować notatki.

<img width="500" height="500" alt="6" src="https://github.com/user-attachments/assets/0fb81f0a-ec89-4807-931c-d424ac2844fb" />

W czasie pisania notatki (tryb source mode lub live preview) możemy używać znaczników Markdown (język znaczników służący do prostego formatowania tekstu za pomocą znaków specjalnych).     

Przykładowa składnia Markdown: https://help.obsidian.md/syntax

### Tagi

Tagi w obsidianie umożliwianie grupowanie notatek wdg. tagów oraz wyszukiwanie po nich: https://help.obsidian.md/tags

### Zapis notatki do pliku

Sporządzone notatki można wyeksportować do pliku pdf - bez dodawania żadnych pluginów (1 i 2).     
Jeżeli chcemy eksportwoać do pliku np. w formacie *.doc należy doinstalować odpowiedni plugin - np. Pandoc.

<img width="500" height="500" alt="5" src="https://github.com/user-attachments/assets/d1e23f7d-a4bf-4af9-b389-532272ac048f" />


### Graf powiązań

Jeżeli w danej notatce znajduje się odniesienie do innej notatki zostaną one połączone na grafie.	
Powiązanie poprzez znacznik [[Example]].

<img width="500" height="500" alt="7" src="https://github.com/user-attachments/assets/e325c0e7-5ad8-4a17-9b5c-a1581d689764" />

Co wynikowo, po kliknięciu w symbol grafu(1) da taki graf powiązań.

<img width="500" height="500" alt="8" src="https://github.com/user-attachments/assets/936248da-052f-4cfe-a0b9-f04f87932436" />



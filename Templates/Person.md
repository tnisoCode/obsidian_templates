<%*
/* 
Kod do automatycznego tworzenia notatek powiązanych - szablonów i zagnieżdżeń szablonów.

Powiązane z tym szablonem templatki zagnieżdżone będą wskazane w treści komentarzem (%%).

Aby utworzyć notatkę z tego Template:

* zainstalować wtyczkę Templater, wskazać folder gdzie znajdują się templatki, wyłączyć folder templatek z wyświetalnia w grafie
* prawy klik w dowolnym folderze
* wybrać opcję '<% create new note from the template'
* wskazać plik z Templates
*/

// Poproś użytkownika o tytuł/ nazwę notatki
let mainTitle = await tp.system.prompt("Nazwa notatki (np. Nazwisko Imie):");
await tp.file.rename(mainTitle); ^69fe5a

// Automatyczne tworzenie notatki Socialmedia w połaczeniu z notatką Person
let socialsTitle = "Socialmedia";
let socialsPath = tp.file.folder(true) + "/" + socialsTitle + ".md";
let socialsFile = await app.vault.getAbstractFileByPath(socialsPath);

if (!socialsFile) {
    // 6. Jeżeli jeszcze nie istnieje to utwórz notatkę
    let socialsTemplate = await tp.file.include("[[Socialmedia]]");
    await app.vault.create(socialsPath, socialsTemplate);
}
-%>

## Informacje o celu

Imię: 
Drugie imię: 
Nazwisko: 
Pseudonim | Aka: 

Data urodzenia: 
Miasto urodzenia: 
Kraj urodzenia: 
Obywatelstwo(a): 

Płeć: 
Wzrost: 
Waga: 
Budowa ciała: 
Kolor oczu: 
Kolor skory: 
Kolor włosów: 
Sylwetka: 
Rasa: 
Wyraźne znaki szczególne (blizny, tatuaże): 

Numer paszportu: 
Numer dowodu os.: 

## LOKALIZACJA

Aktualny adres: 
Na mapie Google: 
Inne drugorzędne adresy: 

Adresy krewnych: 
Adres partnera: 

Adresy przyjaciół i kontaktów: 

Miejsca stałego bywania (sport, hobby, bary itp.): 
Inne adresy posiadanych nieruchomosci, budynków, magazynów, przechowalni, garaży: 

## DANE KONTAKTOWE

Numer telefonu stacjonarnego: 
Telefon(y) komórkowy(e): 
Aplikacje mobilne (WhatsApp, Signal, Telegram): 

Adres(y) e-mail: 
Strona(y) internetowa(e): 
Blogi: 
Profile w sieciach społecznościowych:  %%Zagnieżdźony Template%% [[<%- socialsTitle %>]]

## POJAZD

Prawo jazdy T/N: 
Numer prawa jazdy: 

Posiada pojazd T/N: 
Marka pojazdu: 
Model i kolor pojazdu: 
Tablica rejestracyjna: 
Rok: 

## INFORMACJE ZAWODOWE

Nazwa firmy: 
Strona internetowa firmy: 
NIP firmy: 
Adres firmy: 

## KREWNI

Imię matki: 
Imię ojca: 
Bracia/ Siostry: 
W związku z: 
Żonaty/ zamężna z: 
Liczba dzieci: 
Imiona dzieci: 

## HISTORIA KARALNOSCI

Karany T/N : 
Popełnione przestępstwo(a): 
Uznany za niebezpiecznego T/N: 
Problemy ze zdrowiem psychicznym: 
Możliwie uzbrojony T/N: 
Legalne licencje na broń palną T/N oraz numer licencji i stan: 
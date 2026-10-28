# 🎵 Studio Persona — Dedykowana piosenka na prezent

Cześć! To jest kod źródłowy landing page'a dla **Studio Persona** ([studiopersona.pl](https://studiopersona.pl/)). 

Strona służy do zamawiania spersonalizowanych piosenek na prezent — na urodziny, rocznice, śluby czy podziękowania. Użytkownik podaje swoją historię, a na tej podstawie powstaje unikalny utwór.

---

## 🚀 Co znajduje się na stronie?

Strona to szybki, nowoczesny jednopstronicowy landing page (SPA), na którym użytkownik znajdzie wszystko w jednym miejscu:

* **Odtwarzacz muzyczny (Player):** 
  * Pozwala posłuchać przykładowych piosenek przed zamówieniem.
  * Kręci się na nim płyta winylowa podczas odtwarzania muzyki 🎧.
  * Ma pasek postępu, czas i listę utworów do wyboru.
* **Sekcja „Jak to działa”:**
  * Krok po kroku wyjaśnia proces tworzenia piosenki (od historii po gotowe nagranie).
* **Cennik / Pakiety:**
  * **AIR (49 zł)** – piosenka jako niepubliczny filmik na YouTube.
  * **TAPE (69 zł)** – plik MP3 na własność do pobrania.
  * **PRO (139 zł)** – plik MP3 + dedykowana strona www z odtwarzaczem i galerią zdjęć.
* **Formularz zamówienia:**
  * Dynamicznie zmienia pola w zależności od wybranego pakietu (np. przy pakiecie PRO wyświetla wybór wyglądu strony: *Winyl, Płyta, Kaseta, Polaroidy*).
  * Zbiera dane o osobie, okazji i historii do tekstu piosenki.
  * Posiada zabezpieczenia antyspamowe (honeypot + captcha).
* **Płatności i kontakt:**
  * Formularz po wypełnieniu wysyła zgłoszenie (Web3Forms API) i przekierowuje prosto do bezpiecznej płatności Stripe.

---

## 🛠️ Jak to jest zrobione?

Strona jest lekka, ładuje się błyskawicznie i nie wymaga ciężkich frameworków:

* **HTML5 & CSS3** – autorski wygląd z ciemnym motywem, złotymi akcentami i płynnym menu na telefonach.
* **Czysty JavaScript (Vanilla JS)** – obsługa odtwarzacza audio, przeliczanie czasu, dynamiczne przełączanie pakietów i walidacja formularza.
* **Web3Forms API** – do wysyłania treści zamówienia na maila.
* **Stripe Payment Links** – do obsługi płatności online.

---

## 📁 Struktura plików

* `index.html` – główny kod strony, formularz i odtwarzacz.
* `piosenki-config.js` – lista przykładowych utworów podpinana do odtwarzacza.
* `regulamin.html` & `polityka-prywatnosci.html` – kwestie prawne i RODO.

---

STRONA JEST NIEAKTYWNA
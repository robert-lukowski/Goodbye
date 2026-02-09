# Goodbye App

Interactive web app for collecting farewell messages from a team.
It combines animations, multimedia, and Firebase storage to create a memorable farewell message board.

## English

### What this app does
- Shows a password-protected login screen.
- Opens a main celebration page with animations and music.
- Lets users add farewell wishes.
- Saves and loads wishes in real time using Firebase.
- Optionally redirects to an additional song/video page.

### Features

#### Login
- Animated start screen.
- Password validation.
- Shake effect on invalid password.

#### Main view
- Full-screen background video.
- Parallax and visual effects (glitter, hearts, confetti).
- Intro/join transition.
- Background music.

#### Farewell board
- Form with name and message.
- Live sync with Firebase Realtime Database.
- Wish counter and date-based ordering.

#### Visit metadata
Depending on availability, stored metadata may include:
- country and city,
- IP address,
- browser and operating system,
- device type,
- language.

### File structure
- `index.html` - login screen,
- `main.html` - main page after login,
- `song.html` - optional song/video page,
- `style.css` - app styling,
- `firebase.js` - wish persistence and visit logging,
- `effects.js` - visual effects,
- `parallax.js` - parallax logic,
- `chatbotkam.js` - optional chatbot module,
- media files: `*.mp3`, `*.mp4`, `*.png`.

### Technologies
- HTML5
- CSS3
- JavaScript (Vanilla)
- Firebase Realtime Database
- `canvas-confetti`
- `ipapi.co` (geo-IP)

### Local run
1. Clone the repository.
2. Open `index.html` in your browser.

Note: Firebase and geo/IP features require proper configuration and internet access.

### Firebase configuration
In `firebase.js`, replace the config with your own:

```js
const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  databaseURL: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};
```

### Password configuration
Set your login password in `index.html` (password variable).

### Deployment (GitHub Pages)
1. Push code to GitHub.
2. Go to **Settings -> Pages**.
3. Deploy from the `main` branch (root).

URL format:

`https://<your-username>.github.io/Goodbye/`

## Polska wersja

### Co robi aplikacja
- Pokazuje ekran logowania z hasłem.
- Otwiera stronę główną z animacjami i muzyką.
- Pozwala dodawać życzenia pożegnalne.
- Zapisuje i odczytuje wpisy w czasie rzeczywistym przez Firebase.
- Opcjonalnie przekierowuje do dodatkowej strony z utworem/wideo.

### Funkcje

#### Logowanie
- Ekran startowy z animacją.
- Walidacja hasła.
- Efekt shake przy błędnym haśle.

#### Widok główny
- Pełnoekranowe wideo w tle.
- Parallax i efekty wizualne (glitter, serca, confetti).
- Przejście intro/join.
- Muzyka w tle.

#### Tablica życzeń
- Formularz: imię i wiadomość.
- Synchronizacja na żywo z Firebase Realtime Database.
- Licznik wpisów i sortowanie po dacie.

#### Metadane odwiedzin
W zależności od dostępności mogą być zapisywane:
- kraj i miasto,
- adres IP,
- przeglądarka i system operacyjny,
- typ urządzenia,
- język.

### Struktura plików
- `index.html` - ekran logowania,
- `main.html` - główna strona po zalogowaniu,
- `song.html` - opcjonalna strona z utworem/wideo,
- `style.css` - style aplikacji,
- `firebase.js` - zapis życzeń i logowanie wizyt,
- `effects.js` - efekty wizualne,
- `parallax.js` - logika parallax,
- `chatbotkam.js` - opcjonalny moduł chatbota,
- pliki multimedialne: `*.mp3`, `*.mp4`, `*.png`.

### Technologie
- HTML5
- CSS3
- JavaScript (Vanilla)
- Firebase Realtime Database
- `canvas-confetti`
- `ipapi.co` (geo-IP)

### Uruchomienie lokalne
1. Sklonuj repozytorium.
2. Otwórz `index.html` w przeglądarce.

Uwaga: funkcje Firebase oraz geo/IP wymagają poprawnej konfiguracji i dostępu do internetu.

### Konfiguracja Firebase
W pliku `firebase.js` podmień konfigurację na własną:

```js
const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  databaseURL: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};
```

### Konfiguracja hasła
Ustaw własne hasło logowania w `index.html` (zmienna hasła).

### Deployment (GitHub Pages)
1. Wypchnij kod na GitHub.
2. Wejdź w **Settings -> Pages**.
3. Ustaw deploy z gałęzi `main` (root).

Format adresu:

`https://<twoj-login>.github.io/Goodbye/`

## License

This project was created for a private farewell event.
You can adapt it for your own non-commercial use.

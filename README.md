# Passed Pawn — dokumentacja

**Passed Pawn** to szachowa platforma edukacyjna. **Trenerzy** tworzą kursy złożone z lekcji
(zadania taktyczne, quizy, interaktywne przykłady na szachownicy, wideo), a **uczniowie** je
przeglądają, uzyskują do nich dostęp, uczą się i wystawiają recenzje.

Projekt powstał jako praca dyplomowa (Uniwersytet Gdański, 2025).

## Co jest w tym repo

| Co | Gdzie |
|---|---|
| Pełna dokumentacja (praca dyplomowa, PL): wymagania, UI, architektura, DevOps, AI | [`passed_pawn_documentation_pl.pdf`](passed_pawn_documentation_pl.pdf) |
| Nagrania głównych ścieżek w aplikacji (poniżej) | [`videos/`](videos) |

## Kod źródłowy

| Repozytorium | Zawartość |
|---|---|
| [pp-frontend](https://github.com/passed-pawn-dev/pp-frontend) | Aplikacja SPA dla trenera i ucznia (Angular 19) |
| [pp-backend](https://github.com/passed-pawn-dev/pp-backend) | REST API i logika szachowa (.NET 8, PostgreSQL) |
| [pp-ai](https://github.com/passed-pawn-dev/pp-ai) | Asystent AI w czacie: RAG na dokumentach (FastAPI, LangChain, Chroma, Mistral) |
| [pp-keycloak](https://github.com/passed-pawn-dev/pp-keycloak) | Keycloak z własnym motywem stron logowania i rejestracji |
| [pp-dev-ops](https://github.com/passed-pawn-dev/pp-dev-ops) | Wdrożenie: charty Helm na Kubernetes, pipeline'y CI/CD w Jenkinsie, konfiguracja Keycloaka w Terraformie |

## Nagrania demo

Krótkie filmy (30 s–2 min) nagrane automatycznie Playwrightem. Mają widoczny kursor i napisy
opisujące kolejne kroki (po angielsku). Kliknij miniaturę, żeby otworzyć film.

### Trener — [`videos/coach/`](videos/coach)

| | Film | Co pokazuje |
|---|---|---|
| <a href="videos/coach/e2e_coach.mp4"><img src="videos/thumbnails/e2e_coach.jpg" width="240"></a> | **Pełna ścieżka trenera** · 1:36 | Rejestracja → logowanie → nowy kurs → miniatura → lekcje |
| <a href="videos/coach/create_puzzle.mp4"><img src="videos/thumbnails/create_puzzle.jpg" width="240"></a> | **Zadanie taktyczne** · 0:45 | Tworzenie zadania: pozycja (FEN) + ruchy rozwiązania |
| <a href="videos/coach/create_quiz.mp4"><img src="videos/thumbnails/create_quiz.jpg" width="240"></a> | **Quiz** · 0:55 | Szachownica, pytanie, odpowiedzi, podpowiedź, wyjaśnienie, podgląd |
| <a href="videos/coach/create_example.mp4"><img src="videos/thumbnails/create_example.jpg" width="240"></a> | **Przykład** · 1:27 | Trzykrokowy przykład ze strzałkami i podświetlonymi polami |
| <a href="videos/coach/create_video.mp4"><img src="videos/thumbnails/create_video.jpg" width="240"></a> | **Wideo** · 0:42 | Wgrywanie filmu do lekcji |

### Uczeń — [`videos/student/`](videos/student)

| | Film | Co pokazuje |
|---|---|---|
| <a href="videos/student/e2e_student.mp4"><img src="videos/thumbnails/e2e_student.jpg" width="240"></a> | **Pełna ścieżka ucznia** · 1:56 | Rejestracja → katalog kursów z filtrami → szczegóły kursu (trener, lekcje, recenzje) → darmowy kurs → nauka → recenzja |
| <a href="videos/student/use_puzzle.mp4"><img src="videos/thumbnails/use_puzzle.jpg" width="240"></a> | **Rozwiązywanie zadania** · 0:36 | Błędny ruch zostaje cofnięty, potem poprawne rozwiązanie |
| <a href="videos/student/use_quiz.mp4"><img src="videos/thumbnails/use_quiz.jpg" width="240"></a> | **Quiz** · 0:35 | Podpowiedź, zła odpowiedź, reset, dobra odpowiedź |
| <a href="videos/student/use_example.mp4"><img src="videos/thumbnails/use_example.jpg" width="240"></a> | **Przykład** · 0:31 | Przechodzenie przez kolejne kroki przykładu |
| <a href="videos/student/use_video.mp4"><img src="videos/thumbnails/use_video.jpg" width="240"></a> | **Wideo** · 0:28 | Oglądanie filmu z lekcji |

> Najlepiej zacząć od dwóch pełnych ścieżek (`e2e_coach`, `e2e_student`). Pozostałe filmy
> pokazują po jednym typie elementu lekcji: najpierw jak trener go tworzy, potem jak uczeń z niego korzysta.

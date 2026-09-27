# Passed Pawn — documentation

**Passed Pawn** is an educational chess platform. **Coaches** build courses made of lessons
(tactical puzzles, quizzes, interactive board examples, videos), and **students** browse them,
get access, learn from them and leave reviews.

The project was created as a bachelor's thesis (University of Gdańsk, 2025).

## What's in this repo

| What | Where |
|---|---|
| Full documentation (thesis, in Polish): requirements, UI, architecture, DevOps, AI | [`passed_pawn_documentation_pl.pdf`](passed_pawn_documentation_pl.pdf) |
| Recordings of the main user flows (below) | [`videos/`](videos) |

## Source code

| Repository | Contents |
|---|---|
| [pp-frontend](https://github.com/passed-pawn-dev/pp-frontend) | SPA for coaches and students (Angular 19) |
| [pp-backend](https://github.com/passed-pawn-dev/pp-backend) | REST API and chess logic (.NET 8, PostgreSQL) |
| [pp-ai](https://github.com/passed-pawn-dev/pp-ai) | AI chat assistant: RAG over documents (FastAPI, LangChain, Chroma, Mistral) |
| [pp-keycloak](https://github.com/passed-pawn-dev/pp-keycloak) | Keycloak with a custom theme for the login and registration pages |
| [pp-dev-ops](https://github.com/passed-pawn-dev/pp-dev-ops) | Deployment: Helm charts for Kubernetes, Jenkins CI/CD pipelines, Keycloak configuration in Terraform |

## Demo videos

Short clips (30 s–2 min) recorded automatically with Playwright, with a visible cursor and
captions describing each step. Click a thumbnail to open the video.

### Coach — [`videos/coach/`](videos/coach)

| | Video | What it shows |
|---|---|---|
| <a href="videos/coach/e2e_coach.mp4"><img src="videos/thumbnails/e2e_coach.jpg" width="240"></a> | **Full coach flow** · 1:36 | Registration → login → new course → thumbnail → lessons |
| <a href="videos/coach/create_puzzle.mp4"><img src="videos/thumbnails/create_puzzle.jpg" width="240"></a> | **Puzzle** · 0:45 | Creating a puzzle: position (FEN) + solution moves |
| <a href="videos/coach/create_quiz.mp4"><img src="videos/thumbnails/create_quiz.jpg" width="240"></a> | **Quiz** · 0:55 | Board, question, answers, hint, explanation, preview |
| <a href="videos/coach/create_example.mp4"><img src="videos/thumbnails/create_example.jpg" width="240"></a> | **Example** · 1:27 | A 3-step example with arrows and highlighted squares |
| <a href="videos/coach/create_video.mp4"><img src="videos/thumbnails/create_video.jpg" width="240"></a> | **Video** · 0:42 | Uploading a lesson video |

### Student — [`videos/student/`](videos/student)

| | Video | What it shows |
|---|---|---|
| <a href="videos/student/e2e_student.mp4"><img src="videos/thumbnails/e2e_student.jpg" width="240"></a> | **Full student flow** · 1:56 | Registration → course catalogue with filters → course details (coach, lessons, reviews) → free course → learning → review |
| <a href="videos/student/use_puzzle.mp4"><img src="videos/thumbnails/use_puzzle.jpg" width="240"></a> | **Solving a puzzle** · 0:36 | A wrong move gets reverted, then the correct solution |
| <a href="videos/student/use_quiz.mp4"><img src="videos/thumbnails/use_quiz.jpg" width="240"></a> | **Quiz** · 0:35 | Hint, wrong answer, reset, correct answer |
| <a href="videos/student/use_example.mp4"><img src="videos/thumbnails/use_example.jpg" width="240"></a> | **Example** · 0:31 | Stepping through the example |
| <a href="videos/student/use_video.mp4"><img src="videos/thumbnails/use_video.jpg" width="240"></a> | **Video** · 0:28 | Watching a lesson video |

> Start with the two full flows (`e2e_coach`, `e2e_student`). The other videos each cover one
> type of lesson element: first how the coach creates it, then how the student uses it.

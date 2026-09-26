# Capstone-Project

A planned trivia quiz app powered by a trivia API. The player will be shown questions, earn points for correct answers, and the score (and game) will reset on a wrong answer.

## How it will work

1. The app will fetch a random trivia question from a trivia API.
2. The user submits an answer; a correct answer adds points to the score.
3. An incorrect answer resets the score and starts a new game.

## Tech (planned)

- Trivia question API
- JavaScript

## Getting started

Coming soon — project scaffolding is in progress.

## Planned features

- [ ] Random question fetching with category and difficulty filters
- [ ] Score tracking and best-score persistence
- [ ] Game-over reset flow with play-again option
- [ ] Responsive, accessible quiz UI

## Data source note

The original plan used the jService API (`https://jservice.io`), but that
endpoint no longer responds. A working alternative is the
[Open Trivia Database](https://opentdb.com) (`https://opentdb.com/api.php`),
a free trivia API that supports category and difficulty filters.

Example request:

```text
https://opentdb.com/api.php?amount=1&type=multiple
```

Example response (`response_code` 0 means success):

```json
{
  "response_code": 0,
  "results": [
    {
      "category": "Science: Computers",
      "type": "multiple",
      "difficulty": "easy",
      "question": "What does CPU stand for?",
      "correct_answer": "Central Processing Unit",
      "incorrect_answers": [
        "Central Process Unit",
        "Computer Personal Unit",
        "Central Processor Unit"
      ]
    }
  ]
}
```

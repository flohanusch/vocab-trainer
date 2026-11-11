# Vocab Trainer

Vocabulary flashcards with spaced-repetition practice, speaking practice and Anki export. Single HTML file, no build step, no server.

## Features

- **Practice**: definition → word and fill-the-gap cards, with simple spaced repetition (Again / Good / Easy, six boxes from 10 minutes up to 35 days). Type your answer or just reveal it. Keyboard: `Enter` to reveal, `1` `2` `3` to grade.
- **Words**: search, edit and delete words, grouped by topic. Add new words one at a time, or paste a whole list in the format `word | definition | example with [[word]]`.
- **Use it**: oral-exam practice. Get a discussion question and three target words, answer by typing or speaking (Chrome/Edge), then copy a ready-made prompt to get feedback from Claude.
- **Anki export**: downloads a `.txt` file Anki imports directly, with a Basic card (definition → word) and a Cloze card per word, tagged by topic. Needs Anki 2.1.55+.
- **Backup**: progress lives in the browser's local storage. Download a backup file to move words and progress to another device.

## Adding words with Claude

1. In the **Words** tab, type the new words, one per line, and click **Copy prompt for Claude**.
2. Paste the prompt into Claude. It answers with one line per word.
3. Paste the answer back into the same box and click **Add words**.

## Updating the built-in word list

The starting words are embedded in `index.html` (the `SEED` object). Changing them only affects browsers that haven't opened the app yet; everyone else keeps their saved words and progress. Add new words through the app instead, or load a backup.

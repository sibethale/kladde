# Changelog

## 2026-11-26 (7)
- Added: paste a picture with Ctrl+V instead of uploading it. On an open note it makes a lesson note from the picture. On the New exercise page it makes an exercise from it. Pasting text works as before.

## 2026-11-26 (6)
- Changed: "Add from file" (photos, PDFs, Word, PowerPoint, text) now writes a lesson plan as well. The note starts with a short summary and a numbered study plan with minutes per step, then a section explaining every concept, rule or table in the material (what it is, the rule, Danish examples with translations, exceptions and common mistakes), then words and practice exercises.

## 2026-11-26 (5)
- Fixed: uploading a photo with Groq or OpenRouter ended in "Couldn't reach the AI service", because those AI services can't see photos. Now Kladde reads the Danish text out of the photo on your device (Tesseract OCR, loaded from the internet the first time) and sends only the text. With Claude, photos are still sent directly.
- Changed: when the AI service reports a problem, the message now shows what it said instead of a wrong "check your connection" message.

## 2026-11-26 (4)
- Fixed: in fill-in-the-blank exercises, a blank the AI left without an accepted answer could not be checked ("can't be checked automatically"). Now the app works the missing answer out from the full correct sentence, so those blanks turn green or red and the answer shows in bold.

## 2026-11-26 (3)
- Fixed: in fill-in-the-blank exercises, after pressing Show answer or Check answer, editing a box and then pressing a button (Check answer, Hide answer) sometimes did nothing. The sentence was redrawn as you left the box, which swallowed the click. Now only the colours and message update and the buttons stay put.

## 2026-11-26 (2)
- Added: note categories. Each note has a **Category** box under its title. Type a new name to make a category, or pick an existing one.
- Added: the note list is grouped by category. Click a category title to fold or unfold it, click the pencil to rename it (leave the name empty to remove it), or drag a note onto a category title to move it.
- Changed: search also matches category names.
- Fixed: saving a note keeps its category.

## 2026-11-26
- Added: "Edit with AI" button on an open exercise. Type what to change (for example "make it 12 sentences" or "fix sentence 3") and the AI rewrites the exercise. Your answers so far are cleared.
- Added: optional "Extra instructions for the AI" box when making an exercise from pasted text or a file.
- Added: optional "Extra instructions for the AI" box when letting the AI write a new exercise.

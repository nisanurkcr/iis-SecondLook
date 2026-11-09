# SecondLook

README prose word count: 595 (including headings and lists, excluding this word-count line).

## Project status

SecondLook is an interactive prototype for students using AI coding assistants. It helps them understand a security warning and decide whether to accept a suggested change.

The prototype uses one prepared Python sqlite3 example about SQL injection. The buttons and screen changes work. The warning, explanation and suggested fix are prewritten simulations. No live AI model or security scanner is connected.

Users can:

- Read the warning and open an explanation.
- Compare the original code and suggested fix.
- Accept the change or keep the original.
- Undo an accepted change or restart the example.
- Answer an optional reflection question and receive feedback.

Changes affect only the displayed example. No code is executed, and no user data is saved. The prototype does not check other code or guarantee that an application is secure.

## Technology stack

- HTML provides the page structure.
- CSS controls the appearance and responsive layout.
- JavaScript controls the buttons, displayed code and feedback.
- ChatGPT helped develop the project. The prototype itself does not call ChatGPT or another model.

No dependencies, API keys, backend or installation are needed. A live AI connection is outside the current scope.

## How to run

1. Download the repository using **Code → Download ZIP**.
2. Extract the ZIP.
3. Open `index.html` in a web browser.

You can also inspect the file in VS Code. No localhost server or internet connection is needed after downloading.

## Development record

The following stages took place on 9 November 2026:

- Started with one fixed example to keep the scope manageable. Added explanation, comparison, accept/reject, undo and restart controls.
- Separated the code and warning into panels to make the interaction easier to follow.
- Added a light-hearted introduction, side-by-side comparison and highlighting of the original query. Kept the warning text factual and the simulation labels visible.
- Added optional reflection feedback to help users check their understanding.
- Renamed the project SecondLook and the repository iis-SecondLook.

Automated JavaScript checks passed for the main controls, reflection feedback and reset behaviour. Internal links and control targets were also checked. These checks do not establish usability or security effectiveness. Browser appearance and mobile layout still need manual checking. No user study has been conducted.

## AI assistance

ChatGPT generated the initial HTML, CSS, JavaScript and README. It also revised the interface, suggested names, wrote the introductory text, and drafted the simulated security warning, explanation, fix and reflection feedback.

I requested visual changes and a humorous but serious introduction, selected the design and approved the name SecondLook. ChatGPT applied these revisions. This was substantial assistance, not only grammar correction.

ChatGPT generated and ran JavaScript interaction checks. An initial JavaScript syntax error was found and corrected before those checks passed. A browser-based check was attempted, but the browser download failed, so browser rendering was not verified through that check.

Before submission, I still need to review the code and security explanation, try all controls in a browser, and record the results. This README does not claim those personal checks are complete. There is no live AI service inside the prototype; its responses are fixed text.

## Repository and submission

Repository: https://github.com/nisanurkcr/iis-SecondLook

README: https://github.com/nisanurkcr/iis-SecondLook#readme

The final submitted commit has not yet been selected. Its SHA must be added to the report when the submission version is ready.

## Additional files

`index.html` contains the complete prototype. The project report, abstract, system diagram and illustrated interaction examples are separate deliverables. They are not included in this version. No additional ZIP is needed to run the repository version.

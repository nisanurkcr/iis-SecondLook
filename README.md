# SecondLook

## Project status

SecondLook is an interactive prototype for students using AI coding assistants. It explores how an interface can help users understand a security warning, inspect a suggested fix and decide what to do.

The prototype contains one prepared Python sqlite3 example about SQL injection. The interface controls work, but the warning, explanation, suggested fix and reflection responses are prewritten. No live AI model, security scanner or automatic code analysis is connected.

Working features:

- Open and close a plain-language explanation.
- Compare the original and suggested code.
- Accept the change or keep the original.
- Undo an accepted change.
- Restart the example.
- Answer an optional reflection question and receive fixed feedback.

Acceptance changes only the displayed example. The Python code is not executed. Users cannot upload or analyse other code. No user responses or decisions are saved persistently. There is no learning or personalisation.

The suggested parameterised query addresses the input-handling issue in this example. It does not establish that an entire application is secure. The Python snippets assume an existing database connection, cursor and table.

## Technology stack

- HTML: page structure.
- CSS: appearance and responsive layout.
- JavaScript: controls, displayed code, interface state and feedback.
- ChatGPT and Google Gemini: development and report assistance, described below.

The prototype requires no dependencies, API keys, backend or installation. It does not call ChatGPT, Gemini or another external service.

## How to run

1. Select **Code → Download ZIP** on GitHub.
2. Extract the downloaded ZIP.
3. Open `index.html` in a browser.

No internet connection is needed after downloading. The source can also be inspected in a text editor.

## Development record

- **Scope:** Selected one fixed SQL injection example to keep development manageable and focus on understanding and user decisions.
- **Review interaction:** Added explanation, comparison, accept, keep original, undo and restart controls.
- **Interface revisions:** Separated code and warning panels, added side-by-side comparison, highlighted the original query and made decision feedback visible.
- **Presentation:** Requested a more attractive interface and an informal introduction. Selected the SecondLook name. Kept simulation labels and factual security explanations visible.
- **Reflection:** Added an optional question with explanatory feedback. Answers are not graded or saved.
- **Checks:** Manually tried the browser controls and reviewed the desktop and narrow-window layouts. Used AI-assisted code and SQL checks, as described below.
- **Report preparation:** Developed the rationale and illustrated interactions alongside the prototype. Used screenshots of the actual interface and reviewed AI suggestions about lecture concepts.

## Checks and limitations

On 15 November 2026, I tried all buttons in Chrome on macOS. I checked the initial state, explanation, comparison, acceptance, keeping the original, undo, restart and reflection. I also narrowed the browser window and confirmed that panels stacked and controls remained usable. This was not a physical mobile-device test.

ChatGPT generated and ran JavaScript interaction checks during development. It later checked the JavaScript syntax and tested the SQL examples separately in a temporary SQLite database. The normal lookup returned the expected record; a crafted input changed the original query's behaviour but was treated as a value by the parameterised query.

The security explanation was checked against the official Python sqlite3 documentation:
https://docs.python.org/3/library/sqlite3.html

These are development checks, not verification performed by the prototype at runtime. No user study was conducted. Improvements in understanding, security decisions or resistance to automation bias have not been demonstrated.

## AI assistance

AI assistance was substantial and included both the prototype and the project report. It was not limited to spelling or grammar correction.

**ChatGPT:** Generated the initial HTML, CSS and JavaScript, drafted and revised this README, suggested project names and revised the interface following my requests. It also drafted the simulated warning, explanation, suggested fix and reflection feedback, and generated and ran development checks.

ChatGPT drafted substantial sections of the report, including the abstract, problem explanation, design rationale, development discussion and limitations. It helped connect design choices to lecture concepts, write interaction screenshot captions and discuss references. I used its drafts and revisions when assembling the report.

**Google Gemini:** Reviewed report text, commented on its relationship to the brief and lecture material, and suggested corrections. Its feedback was compared with ChatGPT's suggestions during revision.

**Claude:** Provided an additional review of the report and repository, including suggestions about consistency, citations, presentation and submission requirements.

**My contribution:** Chose the topic and project scope, requested design changes, selected the appearance and name, manually tested the interface, captured screenshots and assembled the report. I questioned AI suggestions about references and unsupported claims, and used those discussions to revise the work. I remain responsible for the submitted content.

## Repository and submission

Repository:
https://github.com/nisanurkcr/iis-SecondLook

README:
https://github.com/nisanurkcr/iis-SecondLook#readme

Development record:
https://github.com/nisanurkcr/iis-SecondLook#development-record

The submitted commit SHA is recorded in the project report to identify the exact repository version being assessed.

## Additional files

`index.html` contains the complete prototype. The project report includes the illustrated interactions and is submitted separately. It is not included in this repository version. No additional ZIP is needed to run the prototype.

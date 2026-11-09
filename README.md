# SecondLook: security warning prototype

README prose word count: 585 (headings and bullets included; code and commands excluded).

## Project status
An early interactive prototype for Understanding Security Warnings in AI-Assisted Programming. It contains one fixed Python sqlite3 example. The interface works, but the warning, explanation and repair suggestion are manually prepared simulations. No AI model, scanner or external API is connected. This is not a general-purpose security analyser.

Working controls: explanation, suggested-change comparison, accept, keep original, undo and restart. Accept changes only the displayed code. Nothing is executed or stored.

## Technology stack
HTML, CSS and plain JavaScript. No dependencies, API keys, server or installation required. The AI behaviour is simulated using fixed text. A live model remains outside the current scope.

## Run or inspect
Download and extract the project. Open index.html in a web browser. Alternatively, open the folder in VS Code and inspect index.html. An internet connection is unnecessary.

## Interaction walkthroughs
1. Open Explain warning, compare the suggested fix, then accept it. Observe the changed code and decision feedback.
2. Compare the fix and select Keep original. Observe that the original remains and the feedback identifies the unresolved issue.
3. Accept the change, then undo it. Restart restores the initial interface state.

## Development record
Initial prototype, 9 November 2026: selected one fixed example to keep development manageable. Added an explanation on request, explicit user approval before replacing code, and undo. Marked all generated-assistant behaviour as simulated. These are initial design proposals to discuss and relate to the module material.

Checks: an automated JavaScript state-transition check passed for explanation, comparison, accept, reject, undo and restart. This checks interface logic, not browser rendering, usability or security effectiveness. No user evaluation has been conducted.

Visual revision, 9 November 2026: following a request for a more attractive interface, separated the editor and warning into panels, added three review steps and a persistent decision area, and updated the editor status after acceptance. Layout adapts to narrow screens. Re-ran the JavaScript state checks successfully. Browser rendering has not been verified in this environment because the browser download failed; check desktop and mobile appearance manually.

Product-style revision, 9 November 2026: added a light-hearted introduction at the student's request. Kept warning descriptions factual and explicitly labelled the opening illustration as fictional. Added side-by-side comparison, line numbers with original-query highlighting, visible acceptance status, and optional reflection with explanatory feedback. The reflection is not graded or saved. Interface-state checks passed for these controls and reset; internal links and accessible control targets were checked. Visual browser verification and user evaluation are still pending.

Brand revision, 9 November 2026: renamed the prototype SecondLook following the student’s choice. The existing GitHub repository name remains iis-codecheck; it does not need to match the product name.

## AI assistance
ChatGPT prepared the initial HTML, CSS, JavaScript and this README, and revised the visual layout and introductory copy following the student’s requests. It also generated and ran the interface state-transition check. The student should inspect the code, try the interactions, revise the design and record their own checks before submission. No claim is made that the student has already performed those checks.

## Repository and submission
The public repository has been created at https://github.com/nisanurkcr/iis-codecheck. This local revision has not yet been uploaded. Add the final submitted commit SHA to the report after uploading and reviewing the work.

## Additional files
index.html is the complete prototype. The project report, abstract, architecture diagram and illustrated storyboards are separate deliverables and are not included in this starter project.

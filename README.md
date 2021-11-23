# Deliverable 07 - Supabase Dropdown Character Maker

[Buggy Supabase Character Designer](https://github.com/alchemycodelab/buggy-js-character-designer-supabase)



### Live Example:
https://alchemycodelab.github.io/js-character-designer/

![](./assets/character-designer.png)

| User should be able to . . .                                                         |             |
| :----------------------------------------------------------------------------------- | ----------: |
| Visit the deployed pages on GitHub pages, with link in the About section of the Github repo |    1 |

| Events                                                                                |             |
| :----------------------------------------------------------------------------------- | ----------: |
| On the home page (`'/'`), Login and Signup using the login and signup form. On success, redirect to the `/character` page   |        1 |
| Logout by clicking the logout button                                                       |        1 |
| If a non-logged-in user tries to visit the character page, redirect them to the login page | 1 |
| On the character page load, fetch the character from supabase and render their details (including all catchphrases) to the page         |        1 |
| On change of the dropdown, update the character in supabase. Then fetch from supabase to update the UI to show the right image |     1 |
| On click of the catchphrase button, update the character in supabase. Then fetch from supabase to update the UI to show the right image. Note that this will require you to keep track of the state of the catchphrases locally in state. |     1 |
| On any dropdown change, see displayed how many times each dropdown has been changed in the current session (NOT tracked in supabase)   |           1 |

| Functions                                                                                |             |
| :----------------------------------------------------------------------------------- | ----------: |
| ASYNC / IMPURE: `fetchAndDisplayCharacter()` : fetches character and sets the images in the DOM
| ASYNC: `fetchCharacter()` : fetches character for currently logged in user from supabase
| ASYNC: `updateHead(newHead)` : updates head of character for currently logged in user from supabase
| ASYNC: `updateMiddle(newMiddle)` : updates middle of character for currently logged in user from supabase
| ASYNC: `updateBottom(newBottom)` : updates bottom of character for currently logged in user from supabase
| ASYNC: `updateCatchphrases(newCatchphrases)` : updates catchphrases of character for currently logged in user from supabase

# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [X] Able to add feedback
    - [X] Data collected on individual pages & components
    - [X] Click on next takes you to the next page in sequence
    - [X] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [X] Thank you page takes you back to the first view
    - [X] Old Data is cleared on form completion

- Client code:
  - [X]  Individual components for each form part
  - [X]  Redux setup complete
    - [X] Store linked to react with `<Provider>`
    - [ 1/2 X ] Store setup with reducer(s) and logger middleware 
  - [ ] Reducers & Actions Working
    - [X] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [X] Actions have a `type` key, and `payload` if sending data
    - [X] Reducers are returning a new state, or the old state (not mutating)
    - [X] Reducers are using spread correctly (to keep old data, while adding new)
  - [X] Review Component shows at all times with current redux state
  - [X] React-Redux Working
    - [X] Dispatching actions onClick
    - [X] Grabbing data from the redux store with `useSelector`
  - [X] Axios POST request to add feedback


- Server code:   
  - [X] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [X] Multiple git commits showing incremental progress
  - [X] Commits are descriptive of the changes made or feature added 
  - [X] Has .gitignore with node_modules
  - [X] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [ ] Appropriate amount of code comments
  - [X] Code is consistently formatted
- Client
  - [X] Appropriate use of HTML tags
  - [X] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [X] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [X] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [X] redux is updated with new score
  - [X] user can continue on to review page and submit as in Base Mode


- Admin View
  - [X] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [X] Can Delete an entry
    - [ ] User is prompted before deleting
  - [X] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [X] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [X] Deployed to Heroku


## Markdown

```
Hey Dane,

Overall, the app looks really clean and is easy to navigate. I particularly like the simplicity of having
just one reducer and spreading the previous properties of each object into that global state.  I would say that although you understand your code, others may have a hard time without many comments.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | no |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes |
| Views are broken down into components | yes |

---
### Notes:

Great work here, Dane! Looks like the app will let you proceed without an input, though.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes | 44 commits!
| Commits are descriptive of the changes made or feature added | partly |
| Readme file updated | yes |
| Appropriate amount of code comments | partly |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Again, great work with all of this, Dane. Your code could probably use a bit more comments in it in
case others are reviewing your code or modifying it and want to know the fuctionality of the things you
have already set up. For your commits, you had a ton of them, but about half were just a few works and
could potentially apply throughout various timelines in your project.

```

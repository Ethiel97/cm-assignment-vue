# Carb Manager Dev Vue.js Assignment

Welcome to Carb Manager Dev Vue.js Assignment. 
There is also a React version of this assignment.  Both assignments are equally scored, feel free to choose one or the other, whichever you feel more comfortable with.
- [cm-assignment-react](TODO://add.cm-assignment-react.link)

## Project structure

The project consists of 2 main modules:
- `node.js` backend: 
  - Express server listening on `http://127.0.0.1:8080`.
  - `http://127.0.0.1:8080/recipes` - returns recipes list. 
  - `http://127.0.0.1:8080/recipe/:id` - returns a single recipe. 
  - `http://127.0.0.1:8080/user` - returns user settings object.
  - Data for all endpoints is mocked.
  - Feel free to modify all files under the `./server` directory except data mocks and corresponding interfaces.
- front-end application:
  - The dev sever listens on `http://localhost:3000`
  - `http://localhost:3000/recipes` - renders recipes list
  - `http://127.0.0.1:8080/recipe/:id` - renders a single recipe
  - Feel free to modify anything

## The challenge

The project contains some poor code. The challenge is to identify the bad parts and address the issues.

- Focus only on the `RecipesView.vue` component.
- `energy` values should be converted based on `user.units.energy` settings. 
- `energy` label should also respect `user.units.energy` settings.
- Assume that all `Recipe.tags` and `Recipe.nutrients` properties are going to be localized based on `User.language`. Don't develop localization code. Just be prepared for it.
- Assume that all `Recipe.nutrients` can be displayed in units based on user settings, which differ from the units provided with the recipe data. Don't develop converters, just be prepared for it.
- Assume that this project is a part of a large-scale application. Recipes are used all over the app, they are not just a property of the `/recipes` page.

- The `/recipe/:id` page just demonstrates that every recipe will use the same recipe model and will require the same problems to be solved.
We don't expect you to write any code for a single recipe view, but we'd like you to have it in mind that such a view will be developed in the future.
- Search for `TODO` and `FIXME` comments and address these issues.
- Feel fee to use TypeScript or JavaScript
- Feel free to create as many components/modules as you want
- Feel free to install any library/tool you need
- Feel free to use Vuex/Pinia
- Feel free to use Composition API or Options API
- Feel free to change the project settings (Vue config, Webpack settings, linters, etc)
- Feel free to contact us any time if you have any questions about the assignment!

We're not aiming for perfection. We don't want you to spend too much time on the refactor.
If a feature/change you'd like to implement is going take too much time just leave your comments in the **Refactor notes** section below.
Include the reason for the refactor and the proposed solution. Also, document all the changes you made e.g.:

- *"Refactored `<Button>` component props to make it re-usable"*
- *"TODO: Define custom validators for all `<Button>` component props"*

We suggest you don't spend more than 2h on this challenge.

## Refactor notes

- `{note_1}`
- `{note_2}`
- `…`
- `{note_n}`

## Submission

- **Clone** the repo (don't fork) to get started. 
- Create a new branch
- Commit all the changes to the new branch
- Create a PR to `main` when you're done

## Customize configuration

This project was set up with [`create-vue`](https://github.com/vuejs/create-vue).
See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Run the express server and serve the front-end app for Development

```sh
npm run serve
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```

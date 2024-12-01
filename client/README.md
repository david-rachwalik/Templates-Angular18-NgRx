# Templates-Angular18-NgRx (Client)

## Web App ([repo](https://github.com/david-rachwalik/Templates-Angular18-NgRx))

Demonstration site for [NgRx](https://ngrx.io) (Reactive State for Angular).&nbsp; NgRx is a state management library based on Redux.

- **[Store](https://ngrx.io/guide/store):** Centralized state container
- **Actions:** Events that describe a state change
- **Reducers:** Pure functions to handle actions and update the state
- **Selectors:** Functions to query the store

### Project Tech Stack

_Languages:_ HTML, CSS, JavaScript, SCSS, TypeScript

Angular, Angular Material, NgRx (data store, redux)

---

### Common Project Commands

Ensure that Docker is running.&nbsp; When the project is opened in VS Code, open the **Command Palette** (`Ctrl+Shift+P`) and select **Dev Containers: Reopen in Container** (or select **Dev Containers: Rebuild and Reopen in Container** if using for the first time).

#### Dev Container Commands

List running containers (shows IDs and names)

```bash
docker ps
```

Connect to container by ID or name

```bash
docker exec -it --user vscode -w /workspaces/<project-name> <container-id> /bin/zsh
```

#### Angular 'generate' Commands Used

Generate a new Angular module

```bash
npm run ng -- g m <module-name>
```

Generate a new Angular component

```bash
npm run ng -- g c <component-name>
```

Example of generating a Blog section

```bash
npm run ng -- g m modules/blog --module=app --route=blog --routing
npm run ng -- g c modules/blog/pages/blog --module=blog
npm run ng -- g c modules/blog/pages/blog-post --module=blog
```

---

---

### Project Creation Commands Used

Generate a new Angular application ([tutorial](https://angular.io/tutorial/toh-pt5), [layouts](https://indepth.dev/posts/1235/how-to-reuse-common-layouts-in-angular-using-router-2))

```bash
ng new <app-name>
```

Install [NgRx](https://ngrx.io) for state management

```bash
npm run ng -- add @ngrx/store --minimal=false --statePath=core/store
npm run ng -- add @ngrx/store-devtools --skip-confirmation
npm run ng -- add @ngrx/entity --skip-confirmation
npm run ng -- add @ngrx/data --defaultCollection --skip-confirmation
npm run ng -- add @ngrx/effects --skip-confirmation
```

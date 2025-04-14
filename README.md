# Day 1

## 🟢 **Beginner Level: Foundations**
### 1. **Prerequisites**
- ✅ HTML, CSS
- ✅ JavaScript (ES6+): `let/const`, arrow functions, promises, destructuring, spread/rest operators
- ✅ TypeScript basics: interfaces, classes, types, generics

### 2. **Environment Setup**
- Install Node.js + npm
- Install Angular CLI:  
  ```bash
  npm install -g @angular/cli
  ```
- Create a project:  
  ```bash
  ng new my-app
  cd my-app
  ng serve
  ```

### 3. **Core Angular Concepts**
- Components
- Templates & Data Binding (interpolation, event binding, property binding, two-way binding)
- Directives (`*ngIf`, `*ngFor`, `ngClass`, `ngStyle`)
- Pipes (built-in & custom)

<!-- ---

## 🟡 **Intermediate Level: Structure & Services**
### 4. **Modules & Routing**
- Feature modules
- Lazy loading
- Route guards (`CanActivate`, `CanDeactivate`)
- Nested routes
- RouterLink and router-outlet

### 5. **Services & Dependency Injection**
- Creating and injecting services
- Singleton vs multi-instance services
- `HttpClient` for API calls
- Observables & RxJS basics (`Observable`, `Subject`, `BehaviorSubject`)

### 6. **Forms**
- Template-driven forms
- Reactive forms
- Form validation (built-in & custom validators)
- Dynamic form controls

### 7. **State Management Basics**
- Using `@Input()` and `@Output()` for parent-child communication
- Shared services for data flow
- RxJS patterns: `switchMap`, `mergeMap`, `debounceTime`

---

## 🔵 **Advanced Level: Architecture & Optimization**
### 8. **Advanced RxJS**
- Higher-order mapping
- Error handling (`catchError`, `retry`)
- Unsubscribing properly (`takeUntil`, `async` pipe)

### 9. **NgRx (Redux pattern)**
- Store, Actions, Reducers, Selectors, Effects
- NgRx DevTools
- Entity adapter
- Async actions with `createEffect`

### 10. **Advanced Angular Concepts**
- Lifecycle hooks (`ngOnInit`, `ngOnDestroy`, etc.)
- Content projection (`ng-content`)
- ViewChild & ContentChild
- Change detection strategies
- Standalone components (Angular 15+)

---

## 🔴 **Expert Level: Performance & Testing**
### 11. **Performance Optimization**
- Lazy loading modules/components
- OnPush change detection
- Virtual scrolling
- TrackBy in *ngFor
- Preloading strategies

### 12. **Testing**
- Unit testing with Jasmine & Karma
- Component testing
- Service testing with mock services
- End-to-end testing with Cypress / Protractor

---

## ⚙️ **Tooling & Best Practices**
- Angular CLI commands (`ng generate`, `ng build`, etc.)
- ESLint / Prettier
- SCSS / Tailwind for styling
- Angular Material / PrimeNG
- Folder structure best practices
- CI/CD with GitHub Actions, Docker, Vercel/Netlify

--> 
---

## 📘 **Resources to Learn**
- [angular.io](https://angular.io) (official docs)
- [RxJS docs](https://rxjs.dev)
- [NG Conf](https://www.ng-conf.org/) & YouTube
<!-- Courses: Udemy (Maximilian Schwarzmüller or Mosh Hamedani), Pluralsight -->

---

# Angular

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 19.2.7.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.

 **modular, scalable Angular folder structure** that supports:

- **Components** (likely reusable UI components)
- **Container pages** (smart components or views/pages)
- **Utils** (static arrays, helper functions, constants)
- **Store management** (NgRx or similar)

Here's an ideal folder structure for your needs, following Angular's best practices and clean architecture principles:

---

## 📁 Suggested Angular Folder Structure

```
src/
└── app/
    ├── core/                         # Singleton services & app-wide logic
    │   ├── services/                 # App-wide services (auth, API)
    │   ├── interceptors/             # HTTP interceptors
    │   ├── guards/                   # Route guards
    │   ├── core.module.ts           # Import once in AppModule
    │   └── index.ts
    │
    ├── shared/                       # Reusable components, pipes, directives
    │   ├── components/               # UI components (buttons, modals)
    │   ├── directives/               # Custom directives
    │   ├── pipes/                    # Reusable pipes
    │   ├── shared.module.ts
    │   └── index.ts
    │
    ├── utils/                        # Static arrays, helper functions, constants
    │   ├── arrays/                   # Static data arrays
    │   ├── helpers/                  # Pure helper functions
    │   ├── constants.ts              # App-wide constants
    │   └── index.ts
    │
    ├── store/                        # State management (NgRx, Signals, etc.)
    │   ├── actions/                  # Global/shared actions
    │   ├── reducers/                 # Global reducers
    │   ├── selectors/                # Global selectors
    │   ├── effects/                  # Global effects
    │   └── app.store.module.ts      # Root store config
    │
    ├── features/                     # Feature-based modules (recommended)
    │   ├── dashboard/                # Feature: Dashboard
    │   │   ├── containers/           # Smart/container components (pages)
    │   │   ├── components/           # Dumb/presentational components
    │   │   ├── store/                # Feature-specific store (actions, reducers, etc.)
    │   │   ├── dashboard.module.ts
    │   │   └── index.ts
    │   │
    │   ├── user/                     # Feature: User management
    │   │   ├── containers/
    │   │   ├── components/
    │   │   ├── store/
    │   │   └── user.module.ts
    │   │
    │   └── ...
    │
    ├── app-routing.module.ts        # Application-level routing
    ├── app.component.ts/html/css    # Root component
    └── app.module.ts                # Root app module
```

---

## 💡 Naming & Structure Philosophy

| Folder          | Purpose                                               |
|-----------------|--------------------------------------------------------|
| `core/`         | App-wide singletons (auth, interceptors, guards)       |
| `shared/`       | Reusable UI components, pipes, directives              |
| `utils/`        | Utility functions, static arrays, constants            |
| `store/`        | Global app-wide NgRx store setup (or signals-based)    |
| `features/`     | Split by business domain with `containers` and `components` |
| `containers/`   | Pages or smart components that connect to store/services |
| `components/`   | Reusable, dumb/presentational UI elements              |

---

## ✅ Example: Static Array & Store Usage

### `utils/arrays/status-options.ts`
```ts
export const STATUS_OPTIONS = [
  { label: 'Active', value: 'active' },
  { label: 'Inactive', value: 'inactive' },
];
```

### `features/user/containers/user-list.component.ts`
```ts
import { STATUS_OPTIONS } from '../../../utils/arrays/status-options';

@Component({ ... })
export class UserListComponent {
  statusOptions = STATUS_OPTIONS;
}
```

### `store/actions/user.actions.ts`
```ts
export const loadUsers = createAction('[User] Load Users');
```

# Generating components

To add a component with a selector `[prefix]-user-list`, run:

```bash
  $ ng g c user-list
  
  installing component
    create src/app/user-list/user-list.component.css
    create src/app/user-list/user-list.component.html
    create src/app/user-list/user-list.component.spec.ts
    create src/app/user-list/user-list.component.ts
    update src/app/app.module.ts
```

> **prefix** prevents element name collisions with components in other apps and with native HTML elements.
So, for example, if prefix is `app` - generated component will have `app-user-list` selector.

- To prevent prefix usage add `--prefix false` or `-p false` flag

```bash
  $ ng g c user-list --prefix false
```

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'user-list',
  templateUrl: './user-list.component.html',
  styleUrls: ['./user-list.component.css']
})
export class UserListComponent {}
```

- To prevent `.spec` files creation add `--spec false` or `-sp false` flag

```bash
  $ ng g c user-list --spec false

  installing component
    create src/app/user-list/user-list.component.css
    create src/app/user-list/user-list.component.html
    create src/app/user-list/user-list.component.ts
    update src/app/app.module.ts
```

- To use inline html templates instead of external templates add `--inline-template` or `-it` flag

```bash
  $ ng g c user-list --inline-template

  installing component
    create src/app/user-list/user-list.component.css
    create src/app/user-list/user-list.component.spec.ts
    create src/app/user-list/user-list.component.ts
    update src/app/app.module.ts
```

- To use inline styles instead of external styles add `--inline-style` or `-is` flag

```bash
  $ ng g c user-list --inline-style

  installing component
    create src/app/user-list/user-list.component.html
    create src/app/user-list/user-list.component.spec.ts
    create src/app/user-list/user-list.component.ts
    update src/app/app.module.ts
```

- To prevent folder creation add `--flat` or `-f` flag

```bash
  $ ng g c user-list --flat
  
  installing component
    create src/app/user-list.component.css
    create src/app/user-list.component.html
    create src/app/user-list.component.spec.ts
    create src/app/user-list.component.ts
    update src/app/app.module.ts
```

You can also combine flags listed above. For example, to create only `.component.ts` file without `.css`, `.html`, `.spec` files and folder use the following command.

```bash
  $ ng g c user-list -f -it -is -sp false
  
  installing component
    create src/app/user-list.component.ts
    update src/app/app.module.ts  
```

All `generate component` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Prevent folder creation         | `--flat`                                | `-f`          | `false`
Prevent prefix usage            | `--prefix false`                        | `-p false`    | `true`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`
Enable  inline html templates   | `--inline-template`                     | `-it`         | `false`
Enable  inline styles           | `--inline-style`                        | `-is`         | `false`

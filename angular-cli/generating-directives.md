# Generating directives

To add a directive with a selector `[prefix]Highlight`, run:

```bash
  $ ng g d highlight

  installing directive
    create src/app/highlight.directive.spec.ts
    create src/app/highlight.directive.ts
    update src/app/app.module.ts
```

- To prevent prefix usage add `--prefix false` or `-p false` flag

```bash
  $ ng g d highlight --prefix false
```

```typescript
import { Directive } from '@angular/core';

@Directive({
  selector: '[highlight]'
})
export class HighlightDirective {}
```

- To prevent `.spec` files creation, use `--spec false` or `-sp false` flag

```bash
  $ ng g d highlight --spec false

  installing directive
    create src/app/highlight.directive.ts
    update src/app/app.module.ts
```

- To prevent folder creation add `--flat` or `-f` flag

```bash
  $ ng g d highlight --flat
  
  installing directive
    create src/app/highlight.directive.spec.ts
    create src/app/highlight.directive.ts
    update src/app/app.module.ts
```

You can also combine flags listed above. For example, to create only `.directive.ts` file without `.spec` file and folder use following command.

```bash
  $ ng g d highlight -f -sp false

  installing directive
    create src/app/highlight.directive.ts
    update src/app/app.module.ts
```

All `generate directive` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Prevent folder creation         | `--flat`                                | `-f`          | `false`
Prevent prefix usage            | `--prefix false`                        | `-p false`    | `true`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`

# Generating Guards

To add a guard called `CanActivateGuard`, run:

```bash
  $ ng g g can-activate

  installing guard
    create src/app/can-activate.guard.spec.ts
    create src/app/can-activate.guard.ts
```

- To prevent `.spec` files creation add `--spec false` or `-sp false` flag

```bash
  $ ng g g can-activate --spec false

  installing guard
    create src/app/can-activate.guard.ts
```

- To enable folder creation add `--flat false` or `-f false` flag

```bash
  $ ng g g can-activate --flat false

  installing guard
    create src/app/can-activate/can-activate.guard.spec.ts
    create src/app/can-activate/can-activate.guard.ts
```

You can also combine flags listed above. For example, to create only `can-activate.guard.ts` file inside `can-activate` folder without `.spec` file use the following command.

```bash
  $ ng g g can-activate -f false -sp false
  
  installing guard
    create src/app/can-activate/can-activate.guard.ts
```

All `generate guard` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Prevent folder creation         | `--flat false`                          | `-f false`    | `true`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`

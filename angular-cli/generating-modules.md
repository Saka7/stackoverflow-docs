# Generating Modules

To add a module called `GuestModule`, run:

```bash
  $ ng g m guest

  installing module
    create src/app/guest/guest.module.ts
```

- To enable `.spec` files creation add `--spec` or `-sp` flag

```bash
  $ ng g m guest --spec

  installing module
    create src/app/guest/guest.module.spec.ts
    create src/app/guest/guest.module.ts
```

- To enable routing use `--routing` or `-r` flag

```bash
  $ ng g m guest --routing

  installing module
    create src/app/guest/guest-routing.module.ts
    create src/app/guest/guest.module.ts
```

You can also combine flags listed above. For example, to create module with routing and specs use the following command.

```bash
  $ ng g m guest -sp -r
  
  installing module
    create src/app/guest/guest-routing.module.ts
    create src/app/guest/guest.module.spec.ts
    create src/app/guest/guest.module.ts
```

All `generate module` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Enable `.spec` files creation   | `--spec`                                |`-sp`          | `false`
Enable routing                  | `--routing`                             |`-r`           | `false`

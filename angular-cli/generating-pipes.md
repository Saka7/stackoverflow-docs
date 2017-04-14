# Generating Pipes

To add a pipe with a name `searchByName`, run:

```bash
  $ ng g p search-by-name

  installing pipe
    create src/app/search-by-name.pipe.spec.ts
    create src/app/search-by-name.pipe.ts
    update src/app/app.module.ts
```

- To prevent `.spec` files creation add `--spec false` or `-sp false` flag

```bash
  $ ng g p search-by-name --spec false
  
  installing pipe
    create src/app/search-by-name.pipe.ts
    update src/app/app.module.ts
```

- To enable folder creation add `--flat false` or `-f false` flag

```bash
  $ ng g p search-by-name --flat false
  
  installing pipe
    create src/app/search-by-name/search-by-name.pipe.spec.ts
    create src/app/search-by-name/search-by-name.pipe.ts
    update src/app/app.module.ts
```

You can also combine flags listed above. For example, to create only `search-by-name.pipe.ts` file inside folder `search-by-name` folder without `.spec` file use the following command.

```bash
  $ ng g p search-by-name -f false -sp false

  installing pipe
    create src/app/search-by-name/search-by-name.pipe.ts
    update src/app/app.module.ts
```

All `generate pipe` flags:

Description                     | Flag                                    | Shortened     | Default Value
---                             | ---                                     | ---           | ---
Enable folder creation          | `--flat false`                          | `-f false`    | `true`
Prevent `.spec` files creation  | `--spec false`                          | `-sp false`   | `true`

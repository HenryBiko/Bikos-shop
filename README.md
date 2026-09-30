# Bikos-shop

A dbt analytics engineering project for the Bikos shop.

> 🚧 **Work in progress.** The project scaffold and example models are in place; shop-specific staging and mart models are next.

## Stack

- **dbt** for transformations, tests, and documentation
- SQL models organized under `models/`

## Project structure

```
Bikos-shop/
├── dbt_project.yml      # project config
├── models/
│   └── example/         # starter models + schema tests
├── analyses/            # ad hoc analytical SQL
├── macros/              # reusable Jinja/SQL macros
├── seeds/               # static CSV reference data
├── snapshots/           # SCD Type 2 history
└── tests/               # custom data tests
```

## Run it

```bash
dbt deps
dbt run      # build models
dbt test     # run schema and data tests
dbt docs generate && dbt docs serve
```

## Author

**Henry Biko** · [GitHub](https://github.com/HenryBiko) · [LinkedIn](https://www.linkedin.com/in/henrybiko)

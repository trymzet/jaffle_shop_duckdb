# Testing dbt project: `jaffle_shop`

`jaffle_shop` is a fictional ecommerce store. This dbt project transforms raw data from an app database into a customers and orders model ready for analytics.

See https://github.com/dbt-labs/jaffle_shop_duckdb for more info.

```shell
git clone https://github.com/trymzet/jaffle_shop_duckdb
cd jaffle_shop_duckdb
uv venv
. .venv/bin/activate
uv install -r requirements.txt
dbt build
dbt docs generate
dbt docs serve
```

To build prod version (with `staging`, `intermediate`, and `marts` schemas), use `--target prod`, eg. `dbt build --target prod`.

## Browsing the data

- [DuckDB CLI](https://duckdb.org/docs/installation/?environment=cli)
- [How to set up DBeaver SQL IDE for DuckDB](https://duckdb.org/docs/guides/sql_editors/dbeaver)

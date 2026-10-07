# PopSQL dbt starter

A minimal dbt project based on [PopSQL's dbt template](https://github.com/popsql/dbt-template).

## Connect in PopSQL

- Repository: `git@github.com:mammadmammadli/test.git`
- Main branch: `main`
- Project subdirectory: leave blank (`dbt_project.yml` is at the root).
- Add the public deploy key shown by PopSQL to this repository's **Settings > Deploy keys**, with **Allow write access** enabled.

After connecting, configure a target under PopSQL's dbt integration settings with your cloud database connection and development schema. PopSQL manages the `default` profile; keep database credentials out of this repository.

Open `models/example/hello_dbt.sql` in PopSQL and preview or compile it. It only selects literal values and needs no source tables. Running `dbt run --select hello_dbt` creates a view named `hello_dbt` in the selected target schema.

The existing query-sync files remain separate from the dbt models.

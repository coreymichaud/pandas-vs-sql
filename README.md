# Hello!

WIP! Still need to create 2 CSV files as tables and complete the notebook.

The data for this notebook was taken from [Bike Store Relational Database | SQL](https://www.kaggle.com/datasets/dillonmyrick/bike-store-sample-database?select=customers.csv) on [Kaggle](https://www.kaggle.com).

# Setup

First, clone this repository to your computer.
```{bash}
git clone https://github.com/coreymichaud/pandas-vs-sql.git
```

Once you're in the repository, install the requirements.
```{bash}
pip install -r requirements.txt
```

# FAQ

Are people actually frequently asking me questions? No... but this section is intended to explain why I structured the notebook the way I did.

### Why DuckDB?

There are many ways to run SQL in Python, but using DuckDB seemed like the easiest way to treat CSV files as database tables and excecute SQL queries. DuckDB also has a very close syntax to PostgreSQL, so all SQL in the notebook should work with Postgres.

### Why no LeetCode style questions?

The notebook is intended to show comparisons between pandas and SQL rather than to show solutions for LeetCode style problems in each syntax.

### Why do the DuckDB queries have .df() at the end?

If you don't include ```.df()``` at the end, the output will look different than the pandas output. Putting it at the end makes each output the exact same for easier output comparison.

### Why are you using CSV files instead of an actual database with tables?

I felt like it was a little easier to use CSV files for this project, and the DuckDB implementation allows me to treat the files like tables. Using CSVs also allows you to view the data files easier, versus a ```.db``` database file which would require database software to view.
# Introduction

Project for learning basic dbt implementation with snowflake

## Getting started

First Install uv to launch virtual invironment

```bash
pip install uv
```
Note: By default pip comes with which Python 3.4 and Python 2.7.9

Then create and activate virtual environment using uv

```bash
uv venv
.venv\Scripts\activate
```

Then install dbt-core and dbt-snowflake to work with it

```bash
pip install dbt-core dbt-snowflake
dbt --help
```

## Development

Go to the directory in terminal where you want to build the project
To Initialize a project use following dbt command

```bash
dbt init
```

Then you will be asked following things answer them correctly
Give project Name - Select which databse you want to chose based on available installed database
Enter acount Identifier - taken value from snowflake credentials from ViewACoount tabl
Enter username - Your snowflake username
Enter password - Your snowflake account password
Enter role - ACCOUNTADMIN
warehouse - transforming (matches with the dbt docs)
database - Analytics (matches with the dbt docs)
schema - dbt_schema
thread - 1

## dbt DOcs 
dbt command to generate doc

```bash
dbt docs generate
dbt docs 
```

## Other 
For dbt command help use below command
```bash
dbt --help
```

Follow steps along [Quickstart guide](https://docs.getdbt.com/guides/snowflake?step=1) for learning dbt

## Acknowledgments

Special Thanks for [dbt Labs](https://docs.getdbt.com/) for providing detailed process on [Quickstart guide](https://docs.getdbt.com/guides/snowflake?step=1) on dbt and Snowflake

Special thanks to the YouTube channel [BugBytes](https://www.youtube.com/@bugbytes3923) for their helpful video tutorial: ["Dagster Tutorial"](https://youtu.be/sKqDq4TFbmY?si=z9qTLQ1BuGLl1LWB).
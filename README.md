# Basic dbt Project

## 📌 Overview
This project is designed for learning the basic implementation of dbt (data build tool) with Snowflake. It provides a hands-on approach to understanding dbt's capabilities in data transformation and modeling.

**Key Features:**
* **dbt Integration:** Learn how to use dbt with Snowflake for data transformation.
* **Virtual Environment Setup:** Use `uv` to manage Python virtual environments.
* **Documentation Generation:** Generate and view dbt documentation.

## 🛠 Tech Stack
* **Language:** Python 3.4+
* **Transformation Tool:** dbt Core
* **Database:** Snowflake

## 🚀 How to Run

### Prerequisites
* Python installed (version 3.4 or higher).
* Snowflake account credentials.

### Steps

1. **Install `uv` to manage virtual environments:**
    ```bash
    pip install uv
    ```
    *Note: By default, `pip` comes with Python 3.4 and Python 2.7.9.*

2. **Create and activate a virtual environment:**
    ```bash
    uv venv
    .venv\Scripts\activate
    ```

3. **Install dbt-core and dbt-snowflake:**
    ```bash
    pip install dbt-core dbt-snowflake
    dbt --help
    ```

4. **Initialize a dbt project:**
    ```bash
    dbt init
    ```
    Follow the prompts to configure the project:
    * **Project Name:** Provide a name for your project.
    * **Database Selection:** Choose Snowflake.
    * **Account Identifier:** Use the value from your Snowflake credentials.
    * **Username:** Your Snowflake username.
    * **Password:** Your Snowflake account password.
    * **Role:** ACCOUNTADMIN
    * **Warehouse:** transforming (matches with the dbt docs)
    * **Database:** Analytics (matches with the dbt docs)
    * **Schema:** dbt_schema
    * **Thread:** 1

## 📊 Documentation

Generate and view dbt documentation using the following commands:
```bash
dbt docs generate
dbt docs
```

## 🛠 Additional Commands

For help with dbt commands, use:
```bash
dbt --help
```

Follow the steps in the [Quickstart guide](https://docs.getdbt.com/guides/snowflake?step=1) to learn dbt.

## 📚 Acknowledgments

Special thanks to:
* [dbt Labs](https://docs.getdbt.com/) for their detailed [Quickstart guide](https://docs.getdbt.com/guides/snowflake?step=1) on dbt and Snowflake.
* The YouTube channel [BugBytes](https://www.youtube.com/@bugbytes3923) for their helpful video tutorial: ["dbt Tutorial"](https://www.youtube.com/watch?v=C9wEdUjTNk8).
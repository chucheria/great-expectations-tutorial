# Great Expectations Tutorial
Code snippets to try the Great Expectations Library

```commandline
pip install great_expectations
great_expectations init
```

After running the init command, your great_expectations directory will contain all of the important components of a local Great Expectations deployment. This is what the directory structure looks like

great_expectations.yml contains the main configuration of your deployment.
The expectations directory stores all your Expectations as JSON files. If you want to store them somewhere else, you can change that later.

The plugins/ directory holds code for any custom plugins you develop as part of your deployment.
The uncommitted/ directory contains files that shouldn’t live in version control. It has a .gitignore configured to exclude all its contents from version control. The main contents of the directory are:
uncommitted/config_variables.yml, which holds sensitive information, such as database credentials and other secrets.
uncommitted/data_docs, which contains Data Docs generated from Expectations, Validation Results, and other metadata.
uncommitted/validations, which holds Validation Results generated by Great Expectations.
# wcraas_docs

Generic project documentation; source of wcraas.github.io repo

## Setup

- Create the following folder structure (as suggested by [MkDocs docu](https://www.mkdocs.org/user-guide/deploying-your-docs/#organization-and-user-pages)):

```
wcraas_docs/
    docs/
    mkdocs.yml
wcraas.github.io/
```

- Create a virtual environment and install the theme requirements:

```sh
$ mkvirtualenv -p $(which python3) wcraas.github.io
$ pip install -r requirements.txt
```

## Deploy

- Navigate to the target repo (`wcraas.github.io`) and trigger deploy:

```sh
cd ../wcraas.github.io
mkdocs gh-deploy --config-file ../wcraas_docs/mkdocs.yml --remote-branch master
```

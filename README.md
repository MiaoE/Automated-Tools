# Automated-Tools
## Description
This repository contains CI/CD tools that can possibly be used in other projects and applications. 

---

### Reference these workflows
#### Pylint
```
name: "Pylint"

on:
  create:
    paths:
      - '**.py'

jobs:
  job-pylint:
    uses: MiaoE/Automated-Tools/.github/workflows/pylint.yml@latest
    with:
      config-file-path: '(optional) the root relative path to pylintrc file'
```
#### Groovy lint
```
name: "Groovy Lint"

on:
  create:
    paths:
      - '**.groovy'
      - '**.gradle'
      - '**.jenkinsfile'

jobs:
  job-groovy-lint:
    uses: MiaoE/Automated-Tools/.github/workflows/groovy-lint.yml@latest
```

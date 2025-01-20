# gitHubActionsVersions

like regexManagers:githubActionsVersions, but matches any (alphanumeric) key or
array item. The datasource and depName tags are required; packageName,
versioning, and extractVersion are optional. Examples:

```
      # renovate: datasource=python-version depName=python versioning=python
      python-version: "3.13"
```

```
    strategy:
      matrix:
        python-version:
          - "3.10"
          # renovate: datasource=python-version depName=python versioning=python
          - "3.13"
```

# dockerfileVersions

Updates build and env variables of the form

```
# renovate: datasource=pypi depName=poetry versioning=pep440
ARG POETRY_VERSION=1.8.3
```

found in Dockerfiles

# gitHubActionsVersions

like regexManagers:githubActionsVersions, but also matches keys of the form `default:`, `foo-version:` and `version:` in addition to `FOO_VERSION:`

# dockerfileVersions

Updates build and env variables of the form

```
# renovate: datasource=pypi depName=poetry versioning=pep440
ARG POETRY_VERSION=1.8.3
```

found in Dockerfiles

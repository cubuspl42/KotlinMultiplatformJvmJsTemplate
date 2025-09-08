# KotlinMultiplatformJvmJsTemplate

This is a [Copier](https://copier.readthedocs.io/) template for a [Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform.html) GitHub-hosted project supporting JVM and JS targets.

## Generating a new project

Export the `PROJECT_OWNER` variable. This might be put in the user's shell initialization script.

This variable will be used in the generated URLs.

```sh
export PROJECT_OWNER=cubuspl42
```

Export the `PROJECT_NAME` variable.

```sh
export PROJECT_NAME=Project1
```

Ensure that the current working directory is the desired **parent** directory for the project.

Generate the project:

```sh
copier copy gh:cubuspl42/KotlinMultiplatformJvmJsTemplate $PROJECT_NAME -d project_owner=$PROJECT_OWNER -d project_name=$PROJECT_NAME --trust
```

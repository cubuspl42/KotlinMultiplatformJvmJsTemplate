# KotlinMultiplatformJvmJsTemplate

This is a [Copier](https://copier.readthedocs.io/) template for a [Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform.html) GitHub-hosted project supporting JVM and JS targets.

## Generating a new project

Export the `PROJECT_OWNER` variable (GitHub user / organization name). This might be put in the user's shell initialization script. Example:

```sh
export PROJECT_OWNER=cubuspl42
```

Export the `PROJECT_NAME` variable (project and repostiory name). Example:

```sh
export PROJECT_NAME=Project1
```

Ensure that the current working directory is the desired **parent** directory for the project.

Generate the project:

```sh
copier copy gh:cubuspl42/KotlinMultiplatformJvmJsTemplate $PROJECT_NAME -d project_owner=$PROJECT_OWNER -d project_name=$PROJECT_NAME --trust
```

Publish the generated project using [`gh`](https://cli.github.com/manual/gh_repo_create):

```sh
git init && gh repo create $PROJECT_OWNER/$PROJECT_NAME --public --source=.
```

Follow the hints in the `Recommended repository setup` section of the generated `README.md` file to configure the created repository reasonably. You may consider removing that section later.

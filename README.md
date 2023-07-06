# Welcome to your CDK TypeScript project

This is a blank CDK project to rebuild trouble with super-linter and ts-standard linting.

## How to setup

```
git init
cdk init app --language=typescript
git add -A
git commit -m 'initial commit'
```

### This setup works fine

```
docker run -e RUN_LOCAL=true -e VALIDATE_TYPESCRIPT_STANDARD=true -v .:/tmp/lint github/super-linter:v4.9.0
```


### This setup does not work

```
docker run -e RUN_LOCAL=true -e VALIDATE_TYPESCRIPT_STANDARD=true -v .:/tmp/lint github/super-linter:v5.0.0
```
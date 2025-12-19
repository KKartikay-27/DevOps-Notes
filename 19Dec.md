# 19th December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/379/753/original/001IntroductionToGitHubActions.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20260203%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20260203T171751Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=f7c57561b3f7ca9e8b03f88b86e3edfc6a48654ee83cba4e0d966e3bfb22e101)


### GitHub Actions
- Built-in CI/CD tool in GitHub

## Key Features
- Workflow automation using YAML
- Large marketplace of reusable actions

## GitHub Actions Basics
### Workflow Files
- Stored in:
  - `.github/workflows/`
- Written in YAML

### Workflow Structure
- **name** – Workflow name
- **on** – Trigger events (push, pull request, etc.)
- **jobs** – One or more jobs
- **steps** – Commands or actions inside a job

## Jobs & Runners
- Each job runs on a runner
- Common runners:
  - `ubuntu-latest`
  - `windows-latest`
  - `macos-latest`
- Ubuntu is most commonly used

## Actions
- Reusable units of work
- Examples:
  - Checkout code
  - Set up language/runtime
- Can use community or custom actions

## Using Maven with GitHub Actions
- Set up Java using `setup-java`
- Run Maven commands:
  - `mvn package`
  - `mvn test`
- pom.xml controls build and dependencies
- Dependency caching improves build speed

## Cost & Execution
- Long-running workflows increase cost
- Stop unused runners
- Keep workflows efficient

# Contributing

Thanks for taking the time to contribute to `terraform-aws-eks-addons`.

## Workflow

1. Fork the repo and create a branch off `main`.
2. Make your change. Keep commits small and follow [Conventional Commits](https://www.conventionalcommits.org/)
   (`fix(scope): short subject` — the `fix` type is required by this repo's PR validation).
3. Run `pre-commit run --all-files` locally so terraform-fmt / tflint / terraform-docs
   all pass before you open a PR.
4. Open a PR against `main`. Label it `bug` (required by this repo's PR validation).
5. CI will validate format, lint, examples, and docs. Once green, a maintainer
   will review.

## Running the examples

Each directory under `examples/` is a standalone Terraform root. `cd` into one,
`terraform init`, `terraform plan`, and you should see a plan with no errors.

## Reporting issues

Use GitHub Issues. If it's a CI / workflow problem, the `review-agent` bot may
have already filed a `[workflow-bug]` ticket — check the existing issues first.

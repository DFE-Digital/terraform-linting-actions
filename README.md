# Terraform Linting Actions

This GitHub workflow will initialise terraform and run validate, fmt, tfdocs, tflint, and checkov.

## Usage

```yml
  terraform-validate
    name: Terraform Lint and Validate
    runs-on: ubuntu-24.04
    steps:
      - uses: DFE-Digital/terraform-linting-actions/.github/actions/terraform-validate@v1.0.0
        with:
          terraform_version: '1.7.0'
          tflint_version: '0.50.3'
          entrypoint: './terraform'
```
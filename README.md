# sample-infra-terraform

Part of the ForeCode test estate. Not a real product.

Shared AWS infrastructure in Terraform. Every change is formatted, validated and planned; `staging` is applied on every
change to `main` and on a schedule, `production` when run manually (the `production` environment needs an approval).

Deploys are simulated: `.github/simulate.sh` runs `terraform init` without a backend and makes `plan` and `apply`
print what they would do.

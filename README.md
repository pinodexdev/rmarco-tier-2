# DevOps Technical Challenge Tier 2

## Naming Convention

`project-name-environment-resource-name`

* Resource names should use `kebab-case`
* Resource names should be prefixed with the project name and environment

### Examples

* `store-dev-vpc`
* `store-dev-ecs-instance`
* `store-dev-master-db`
* `store-prod-vpc`
* `store-prod-ecs-instance`
* `store-prod-master-db`

## Tags

Each resources must have the following tags:

* **Name** - resource name which is usually displayed in the table
* **Project** - project name that the resource belongs to
* **Environment** - environment name that the resource belongs to

Tag values must also follow the naming convention specified above.

## Stack Creation Order

1. [rmarco-tier-2-vpc.yml](rmarco-tier-2-vpc.yml)
2. [rmarco-tier-2-rds.yml](rmarco-tier-2-rds.yml)
3. [rmarco-tier-2-ecs.yml](rmarco-tier-2-ecs.yml)
4. [rmarco-tier-2-cicd.yml](rmarco-tier-2-cicd.yml)
5. [rmarco-tier-2-cloudfront.yml](rmarco-tier-2-cloudfront.yml)

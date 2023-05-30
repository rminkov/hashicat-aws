# hashicat-aws
Hashicat: A terraform built application for use in Hashicorp workshops

Includes "Meow World" website.

[![infrastructure-tests](https://github.com/hashicorp/hashicat-aws/actions/workflows/infrastructure-tests.yml/badge.svg)](https://github.com/hashicorp/hashicat-aws/actions/workflows/infrastructure-tests.yml)

-----------

If you want to use Terraform CLoud as a remote backend add this file: remote_backend.tf

```
terraform {
  backend "remote" {
    hostname = "app.terraform.io"
    organization = "YOURORGANIZATION"
    workspaces {
      name = "hashicat-aws"
    }
  }
}
```

---------------

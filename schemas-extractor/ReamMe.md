Simple utility to get schemas of all official Terraform Providers

How to Use
-----

1. Ensure you have `GOPATH` env variable set up

2. Run `make`

3. If Check providers failed, you need to append "providers.base.new.json" entries to "providers.base.json"

4. If Cloning failed, remove entry in "providers.base.json" and rerun make

5. You'll see `schemas` directory with schemas and 'failure.txt' file with list of failed providers
6. Copy all json files from `schemas` directory to `/REPO_ROOT/terraform/model/providers/`
7. Copy providers.list to `/REPO_ROOT/terraform/model/`


8. Call update-list-files.sh to update files .list under terraform/model

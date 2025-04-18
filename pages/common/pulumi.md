# pulumi

> Define infrastructure on any cloud using familiar programming languages.
> Some subcommands such as `up` have their own usage documentation.
> More information: <https://www.pulumi.com/docs/iac/cli/>.

- Create a new project using a template:

`pulumi new`

- Create a new stack using an isolated deployment target:

`pulumi stack init`

- Configure variables (e.g. keys, regions, etc.) interactively:

`pulumi config`

- Preview and deploy changes to a program and/or infrastructure:

`pulumi up`

- Preview deployment changes without performing them (dry-run):

`pulumi preview`

- Destroy a program and its infrastructure:

`pulumi destroy`

- Use Pulumi locally, independent of a Pulumi Cloud:

`pulumi login {{[-l|--local]}}`

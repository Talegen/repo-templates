# @Talegen/repo-templates

> Talegen's default repo templates

The **official, default** template at Talegen is the one called **Apache-2.0**.  If you combine the
files in the `shared/` folder with the files in `projections/Apache`, you get the standard, default
set of files that new GitHub repos are placed with in the company.

## What is this?

These files are packaged as the default, standard recommended content for net new
GitHub repos created by Talegen across all official Talegen GitHub orgs such
as `Talegen`, `Bastille-Id`, etc.

When Talegen creates new repos, either through internal tooling, or on GitHub directly,
these files are applied as sane defaults and help to encourage community.

Please help build the future of Talegen open communities by making thoughtful contributions here.

These projects should be technology-agnostic.

## Talegen template types

The templates today are listed below. **The official, main, primary Talegen template is called "Apache

### issueonly

An "issue-only" repo is a GitHub repository that primarily is used to report bugs, issues, and other
feedback, but not host or store code.

### Apache

The standard, default template for Talegen releases, placing an Apache `LICENSE` file and other
basics.

The `README.md` file has a rich metadata header with required fields and information that is processed
by the docs site. The template outlines some of the files that are placed.

Samples created through this mechanism are also configured automatically with a GitHub webhook that
connects with a sample publishing system.

## Structure of directories

### `shared` directory

The common directory contains defaults that all templates use unless overridden.

### `projections` directory

These are more specific templates for projects

## Output of the union of the directories

```text
// psuedo-code
for (each templateName of projections) {
  copy(sharedFiles, excludingAnySpecialExclusions);
  copy(specificProjectionFiles);
}
```

## Contributing

This project welcomes contributions and suggestions.

### Pull request review

Pull requests to this repo will be reviewed, at a minimum, by Talegen.

Please understand that these templates often need to be kept rather simple, since
they are a starting point, and if there is too much guidance, teams may not be familiar
with how to react and manage projects with too much initial content.

### Contribution requirements

Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit [Contributor License Agreements](https://talegen.com/contributor-license-agreements).

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

## Code of Conduct

This project has adopted the [Talegen Open Source Code of Conduct](https://talegen.com/open-source-code-of-conduct/).
For more information see the [Talegen Code of Conduct FAQ](https://talegen.com/open-source-code-of-conduct-faq/) or
contact [support@talegen.com](mailto:support@talegen.com) with any additional questions or comments.

# Packaging
The packager utility prepares a fully-functional codebase with the docroot one level into the package.

## Usage
The build is executed by the `package` fin command:

    $ fin package

The packaged build artifact is a fully-functional codebase with symlinks to custom code dereferenced and copied in. The output will end up in the `package` directory. This directory is ingored by local git and would normally be the root of the deployment repository.


# Setup Jolie action

Github action for setup Jolie programming language to the Github action runner. It downloads, install, and setup the required system variable to execute Jolie service.

## Usage

- `version`: Jolie version to be setup. It should be corresponding to the release version tag on [Releases](https://github.com/jolie/jolie/releases). default: `v1.11.0`

## Example

```yml
steps:
  - uses: actions/checkout@v3
  - id: setup-jolie
    uses: jolie/setup-jolie@v1
  - run: jolie main.ol
    shell: bash
```

## TODO

- Introduce cache to increase the performance on downloading the installation.

## License

The scripts and documentation in this project are released under the [GNU LESSER GENERAL PUBLIC LICENSE](LICENSE).
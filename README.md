# Set up Jolie

GitHub action for setting up a Jolie programming language environment.

It downloads and installs Jolie, making it possible to execute Jolie services by running the usual `jolie <program.ol>`.

## Usage example

```yml
steps:
  - uses: actions/checkout@v3
  - id: setup-jolie
    uses: jolie/setup-jolie@v1
  - run: jolie main.ol
    shell: bash
```


## Parameters

- `version`: desired Jolie version. See [Jolie releases](https://github.com/jolie/jolie/releases) for available versions. Current default is `1.12.0`. Note that the `v` used in the GitHub tags of Jolie should not be used.
- `java-version`: desired Java version. Current default is `21`.
- `node-version`: desired Node version. Current default is `20`.

## Future work

- Introduce a cache to increase the performance of downloading the Jolie installer.

## License

The scripts and documentation in this project are released under the [GNU LESSER GENERAL PUBLIC LICENSE](LICENSE).

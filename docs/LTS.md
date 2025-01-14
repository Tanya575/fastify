<h1 align="center">Fastify</h1>

<a name="lts"></a>

## Long Term Support

Fastify's Long Term Support (LTS) is provided according to the schedule laid
out in this document:

1. Major releases, "X" release of [semantic versioning][semver] X.Y.Z release
   versions, are supported for a minimum period of six months from their release
   date. The release date of any specific version can be found at
   [https://github.com/fastify/fastify/releases](https://github.com/fastify/fastify/releases).

1. Major releases will receive security updates for an additional six months
   from the release of the next major release. After this period is expired,
   we will still review and release security fixes as long as they are
   provided by the community and they do not violate other constraints,
   e.g. minimum supported Node.js version.

1. Major releases will be tested and verified against all Node.js
   releases that are supported by the
   [Node.js LTS policy](https://github.com/nodejs/Release) within the
   LTS period of that given Fastify release line.

A "month" is to be a period of 30 consecutive days.

[semver]: https://semver.org/

<a name="lts-schedule"></a>

### Schedule

| Version | Release Date | End Of LTS Date | Node.js              |
| :------ | :----------- | :-------------- | :------------------- |
| 1.0.0   | 2018-03-06   | 2019-09-01      | 6, 8, 9, 10, 11      |
| 2.0.0   | 2019-02-25   | 2021-01-31      | 6, 8, 10, 12, 14     |
| 3.0.0   | 2020-07-07   | TBD             | 10, 12, 14, 16       |

<a name="supported-os"></a>

### CI tested operating systems

Fastify uses GitHub Actions for CI testing, please refer to [GitHub's documentation regarding workflow runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-runners-and-hardware-resources) for further details on what the latest virtual environment is in relation to the YAML workflow labels below:

| OS      | YAML Workflow Label    | Package Manager           | Node.js      |
|---------|------------------------|---------------------------|--------------|
| Linux   | `ubuntu-latest`        | npm                       | 10,12,14,16  |
| Linux   | `ubuntu-16.04`         | yarn,pnpm                 | 10,12        |
| Windows | `windows-latest`       | npm                       | 10,12,14,16  |
| MacOS   | `macos-latest`         | npm                       | 10,12,14,16  |

Using [yarn](https://yarnpkg.com/) might require passing the `--ignore-engines` flag.

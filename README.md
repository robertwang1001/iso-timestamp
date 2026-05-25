<h1 align="center">Welcome to iso-timestamp 👋</h1>

![GitHub License](https://img.shields.io/github/license/robertwang1001/iso-timestamp)
![GitHub commit activity](https://img.shields.io/github/commit-activity/w/robertwang1001/iso-timestamp)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/robertwang1001/iso-timestamp/release.yaml)
![GitHub Release](https://img.shields.io/github/v/release/robertwang1001/iso-timestamp)
![GitHub Release Date](https://img.shields.io/github/release-date/robertwang1001/iso-timestamp)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/robertwang1001/iso-timestamp)
![GitHub watchers](https://img.shields.io/github/watchers/robertwang1001/iso-timestamp)
![GitHub forks](https://img.shields.io/github/forks/robertwang1001/iso-timestamp)
![GitHub Repo stars](https://img.shields.io/github/stars/robertwang1001/iso-timestamp)
![NPM Version](https://img.shields.io/npm/v/iso-timestamp)
![NPM Type Definitions](https://img.shields.io/npm/types/iso-timestamp)
![NPM Downloads](https://img.shields.io/npm/dw/iso-timestamp)
![Node Current](https://img.shields.io/node/v/iso-timestamp)

Generate ISO 8601 timestamp: YYYYMMDDhhmmssSSS

## Install

```bash
npm install iso-timestamp
```

or

```bash
yarn add iso-timestamp
```

or

```bash
pnpm add iso-timestamp
```

## API

### `timestamp(options?)` or `timestamp(date, options?)`

  * `date`: Custom date

  * options:
    * `excludeTime`: Exclude time, i.e. hour, minute and second. *Default: false*
    * `excludeMillisecond`: Exclude millisecond from time. *Default: false*
    * `separator`: Separator among elements of the timestamp. *Default: ''*

```typescript
import timestamp from 'iso-timestamp'
// Or import { timestamp } from 'iso-timestamp'

timestamp()
// return current timestamp: 202408070101123

timestamp({ excludeMillisecond: true })
// return timestamp with millisecond excluded: 202408070101

timestamp({ excludeTime: true })
// return timestamp with time excluded: 20240807

timestamp(new Date('2050-03-04T12:03:04.123'), { excludeMillisecond: true })
// return timestamp with custom Date: 20500304120304

timestamp({ separator: '-', excludeTime: true })
// return timestamp with custom separator: 2024-08-07
```

## Contributing

Contributions are welcome! If you have ideas, bug fixes, or improvements, please open an issue or submit a pull request on the
[GitHub repository](https://github.com/robertwang1001/iso-timestamp).

Give a ⭐️ if this project helped you!

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

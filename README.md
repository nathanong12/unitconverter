# Unitconverter

![Master Build](https://img.shields.io/travis/keithalpichi/unitconverter/master.svg?label=build%3A%20master&style=for-the-badge)

![Dev Build](https://img.shields.io/travis/keithalpichi/unitconverter/develop.svg?label=build%3A%20dev&style=for-the-badge)

![NPM Version](https://img.shields.io/npm/v/@keithalpichi/unitconverter.svg?style=for-the-badge)

![Package Size](https://img.shields.io/bundlephobia/min/@keithalpichi/unitconverter.svg?style=for-the-badge)

![License](https://img.shields.io/npm/l/@keithalpichi/unitconverter.svg?style=for-the-badge)

![Stars](https://img.shields.io/github/stars/keithalpichi/unitconverter.svg?style=for-the-badge)

Unitconverter is a library to convert units of measurements such as length, mass, volume, and more. 

If you need to convert inches to centimeters, centimeters to feet, kilograms to pounds, liters to quarts, or perform any other conversions then Unitconverter is the library for you.

It is written in Typescript, compiled to Javascript, and thoroughly tested with Jest.

## Table of Contents

1. [Installation](#installation)
1. [Usage](#usage)
1. [Documentation](#documentation)
1. [Develop](#develop)
1. [Contributing](#contributing)
1. [RoadMap](#roadmap)
1. [Changelog](#changelog)
1. [License](#license)

## Installation

`npm i @keithalpichi/unitconverter`

## Usage
Simply import the type of converter you'd like to use. In this case we'll showcase the `LengthConverter`:
```
const { LengthConverter } from "@keithalpichi/unitconverter"
```

Initialize an instance:
```
const item = new LengthConverter({ unit: "ft", value: 2 });
```

Use the `add` method to add to the converter value:
```
item.add(1); // value is now at 3
```

Use the `to` method to convert the unit to another unit:
```
item.to("in");
```

Use the `value` method to return the converted value
```
item.value(); // 36
```

Additionally, you can chain the methods together:
```
const value = item.add(1).to("in").value();
```

## Documentation

Refer to the [Documentation Guide](./DOCUMENTATION.md)

## Develop

If you're interested in contributing please read the [Contributing Guide](./CONTRIBUTING.md)

* Fork this repo
* Install dependencies with `npm i`
* Create tests for your changes
* Make your changes
* Test your changes with `npm run test` (there is also  a git pre-commit hook that runs this script if you forget to)

## Contributing

Refer to the [Contributing Guide](./CONTRIBUTING.md)

## Roadmap

- Add `MassConverter`
- Add `VolumeConverter`

View the [Issue Tracker](https://github.com/keithalpichi/unitconverter/projects/1) for more details.

## Changelog

Refer to the [Changelog Document](./CHANGELOG.md)

## License

Unitconverter is [MIT licensed](./LICENSE)

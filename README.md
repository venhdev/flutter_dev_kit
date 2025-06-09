<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/tools/pub/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/to/develop-packages).
-->

A development kit for Flutter projects, providing common utilities and extensions.

## Features

- `indentJson`: A utility function to pretty-print JSON strings.
- `stringify`: A utility function to convert various data types to their string representation, handling JSON serialization for Maps and Iterables.

## Getting started

### Installation

Add the following to your `pubspec.yaml` file:

```yaml
dependencies:
  dev_kit: ^0.0.1
```

Then, run `flutter pub get`.

## Usage

```dart
import 'package:dev_kit/dev_kit.dart';

void main() {
  // Example usage of DevKit utilities
  final Map<String, dynamic> data = {
    'name': 'DevKit',
    'version': '0.0.1',
    'features': ['indentJson', 'stringify'],
  };

  print('Indented JSON:');
  print(indentJson(data));

  print('\nStringified value:');
  print(stringify(123));
  print(stringify('hello'));
  print(stringify(data));
}
```

For more examples, please see the `/example` folder.

## Additional information

This package is open-source and contributions are welcome. Feel free to open issues or pull requests on the GitHub repository: https://github.com/venhdev/flutter_dev_kit

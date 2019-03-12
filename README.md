# transparent_image

A simple transparent image. Represented as a Uint8List, which was originally
extracted from the Flutter codebase (was private in the test package).

It's a silly, simple library, but I found I needed transparent images in a few
projects and found this is the simplest way to represent it :)

## Usage

This package exports one constant: `kTransparentImage`.

### Image Widget

Displays the transparent image. 

```dart
Image.memory(kTransparentImage);
```

### FadeInImage Widget

A more useful example, and the reason I originally extracted this from the
Flutter codebase!

A [complete
example](https://flutter.dev/docs/cookbook/images/fading-in-images#in-memory)
can be seen on the Flutter website.

```dart
FadeInImage.memoryNetwork(
    placeholder: kTransparentImage,
    image: 'https://picsum.photos/250?image=9',
  ),
);
```

## Contributors

  * Flutter team
  * Brian Egan
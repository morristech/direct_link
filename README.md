# direct_link

For those who want to create a movie and downloader app, this is a useful package.

You can get a direct link from the URL that my support sites.

## Support Sites
- Vimeo
- Twitter
- Youtube
- Facebook
- DailyMotion
* PCloud
* MegaUp
* Dropbox
* SolidFiles
* MediaFire
* MP4Upload
* Google Drive
- Xnxx
- PornHub
- xHamster


## Getting Started

In the `pubspec.yaml` of your flutter project, add the following dependency:

```yaml
dependencies:
  ...
  direct_link:
```

Next we need to install this

```sh
# Dart
pub get

# Flutter
flutter packages get
```

In your library add the following import:

```dart
import 'package:direct_link/direct_link.dart';
```

## Usage

Use `check` class to check your link have been existed my support sites

```dart
var check = await DirectLink.check(url); // add your url
```

### Example

```dart
if (check == null) {
    // null condition
}else{
     if (check.length > 1) {
         // multiple links and quality
     }else{
         // single link
     }
}

```
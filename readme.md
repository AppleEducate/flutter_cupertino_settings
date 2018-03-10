# flutter_cupertino_settings

![Pub badge](https://img.shields.io/pub/v/flutter_cupertino_settings.svg)  ![](https://img.shields.io/github/license/matthinc/flutter_cupertino_settings.svg)

A Flutter widget to create an iOS settings-table (static TableView).

[Get from Pub](https://pub.dartlang.org/packages/flutter_cupertino_settings#-installing-tab-)

- [x] Basic items (CSHeader & CSControl)
- [ ] Support for icons
- [ ] Dynamic lists
- [ ] Item selection
- [x] Button cells
- [ ] Full width controls

```dart
new CupertinoSettings(<Widget>[
    new CSHeader('Controls'),
    new CSControl('Brightness', new CupertinoSlider(value: 0.5)),
    new CSControl('Auto brightness', new CupertinoSwitch(value: true)),
    new CSHeader(),
    new CSControl('Loading...', new CupertinoActivityIndicator()),
    new CSHeader('Extra'),
    new CSControl('Version', new Text('1.0.0')),
    new CSControl('Author', new Text('Matthias Rupp')),
    new CSButton(CSButtonType.DEFAULT, "Licenses", (){}),
    new CSHeader(),
    new CSButton(CSButtonType.DESTRUCTIVE, "Delete all data", (){})
]);
```

![](http://abload.de/img/untitled5oqr2.png)
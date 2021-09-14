# tutorial
flutter公式チュートリアル(Write your first app)
https://flutter.dev/docs/get-started/codelab

## メモ
テーマデータの変更はチュートリアルでは
```
      theme: ThemeData(          // Add the 3 lines from here...
        primaryColor: Colors.white,
      ),
```
になっているが、プロパティが更新されており、ThemeDataそのものにprimaryColorプロパティは存在しない。
以下で動作
```
      theme: ThemeData(
        colorScheme: ColorScheme.fromSwatch(
            primarySwatch: Colors.amber),
      ),
```
参考: https://api.flutter.dev/flutter/material/ThemeData-class.html
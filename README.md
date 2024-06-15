# Project name: POMODORA TIMER
## Motivation:Want to design a good looking timer
![計時器圖片](photo/timer.png)


### main.dart
```import 'package:flutter/material.dart';
import 'view/countdown-page.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  static final String title = 'CountdownTimer';
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: title,
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: CountdownPage(),
    );
  }
}
```
### round-button.dart
```import 'package:flutter/material.dart';

class RoundButton extends StatelessWidget {
  const RoundButton({
    Key? key,
    required this.icon,
  }) : super(key: key);
  final IconData icon;

  @override
  Widget build(BuildContext context) {
    return Padding(
      padding: const EdgeInsets.symmetric(
        horizontal: 5,
      ),
      child: CircleAvatar(
        radius: 30,
        backgroundColor: Colors.black,
        child: Icon(
          icon,
          size: 36,
          color: Colors.white,
        ),
      ),
    );
  }
}
```
## Reference
- [Countdown timer:Creating a Countdown Timer using Animation in Flutter | by Ashish Rawat | FlutterDevs](https://www.youtube.com/watch?v=bjAsnIw3VCs)

- [Time picker] (https://www.youtube.com/watch?v=gQFRwAvShJc)
- [Background] (https://www.youtube.com/watch?v=eN62zlmjAEQ&t=0s)

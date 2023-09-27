import 'dart:js_util';

import 'package:flutter/material.dart';

void main(){
  runApp(new myApp());
}
class myApp extends StatelessWidget {
  const myApp({super.key});

  @override
  Widget build(BuildContext context) {
    return new MaterialApp(
      title: "Chat App",
      home: new _homepage(),
    );
  }
}
class _homepage extends StatefulWidget {
  const _homepage({super.key});

  @override
  State<_homepage> createState() => _homepageState();
}

class _homepageState extends State<_homepage> {
  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: new Text("Chat App"),
      ),
      body: new Container(
        child: new Row(
          mainAxisAlignment: MainAxisAlignment.end,
          children: [
            new TextField(
              keyboardType: TextInputType.text,
              style: new TextStyle(
                
              ),
            )
          ],
        ),
      ),
    );
  }
}


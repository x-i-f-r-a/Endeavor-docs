# Architecture Support

Endeavor web framework support two type of architecture for developing web applications.

## Express Js Architecture

For the developers from Javascript and for the developers who are developing small API's or websites , Endeavor support Express Js type developing architecture.

#### Example 

```dart

import 'package:endeavor/endeavor.dart';


class App{
  void main({server}) async {
    final app = Endeavor();


    app.GET('/', (Request req, Response res){
        res.sendString('Momentum is up and running');
    });

    app.runServer();

  }
}

```
Or 

```dart

import 'package:endeavor/endeavor.dart';


class App{  
  void main({server}) async {
    final app = Endeavor();


    app.GET('/', Home);


    Future Home(Request req, Response res){
          res.sendString('Momentum is up and running');
    };

    app.runServer();

  }}

```


## Laravel like Architecture


For the web wizards , momentum support separating logic and view. 
The `Controllers` folder contains the sample program to write a separate class with functions and it can be called inside our main `main.dart` file.



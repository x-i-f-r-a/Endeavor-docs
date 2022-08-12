# Basic Authentication

Basic authentication for different routes can be added inside the Momentum class. Example,

```dart
import 'package:endeavor/endeavor.dart';

class App{
  void main({server}) async {

    final app = Endeavor(
        basicAuth: {
            '/': 'username:password'
            '/dashboard': 'username2:password2'
            }
      );


    app.GET('/', (Request req, Response res){

      app.GET('/', (Request req, Response res){
            res.sendString('My Endeavor app');
        });

    });

    app.runServer();
    
  }
}

```
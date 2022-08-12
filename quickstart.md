## Quick Start 

### Prerequisites 

In order to use Endeavor Web Framework you must have the [Dart SDK][dart_installation_link] installed on your machine.


Endeavor requires Dart `">=2.17.0 <3.0.0"`


### Installing Endeavor CLI Tool 

```shell
#  Install the ectl cli from pub.dev

dart pub global activate ectl

```

### Creating a New Project 

Use the `ectl create <project name>` command to create a new project.

```shell
#  Create a new project called "MyDreamProject"
ectl create MyDreamProject
```

The directory structure is as follows:

```text
MyDreamProject
└── app
    └── MyDreamProject.dart
└── templates
    └── Home_view.dart
└── Controllers
    └── Home.dart
├── pubspec.yaml
├── main.dart
└── isolator.dart
```

### Start the Development Server

Next, open the newly directory of created project and start the dev server by:

```shell
#  Start the development server
ectl dev
```


By default port `80` is used. A custom port can be used inside the app's port option.




[dart_installation_link]: https://dart.dev/get-dart
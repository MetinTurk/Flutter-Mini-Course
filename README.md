# Mini Course: Fundamentals of Mobile App Development with Flutter

**Topic:** Introduction to cross-platform mobile app development using the Flutter framework and Dart language.
**Target Audience:** Beginner developers with basic programming knowledge who want to learn how to build iOS and Android applications from a single codebase.

## IDE Customization
* **Code Style Rules & Inspections:** The IDE is customized to enforce a strict 80-character line limit for Dart files and automatically format code using trailing commas. Additionally, the inspection "Prefer `const` with constant constructors" is elevated to a **Warning** to ensure students learn UI performance optimization from the start.

## Unit 1: Introduction to Widgets and State

### Theory Tasks
* **Task 1: Everything is a Widget**
  * *Description Text:* In Flutter, the user interface is built entirely out of widgets. A widget describes what the view should look like given its current configuration and state. When a widget’s state changes, the framework rebuilds it to reflect the new data.
  * *Link:* [Flutter Official Widget Catalog](https://docs.flutter.dev/ui/widgets)
* **Task 2: The Widget Tree**
  * *Description Text:* Widgets are organized in a hierarchical structure called the Widget Tree. The root is typically a `MaterialApp`, branching down to structural layouts (like `Scaffold`, `Column`) and individual UI elements (like `Text`, `Icon`).
  * *Image:* <img width="1408" height="768" alt="MeslekiYabancıDilResim" src="https://github.com/user-attachments/assets/ba775609-8518-4d88-9d57-a396eb179bc9" />
* **Task 3: Stateless vs. Stateful Widgets**
  * *Description Text:* A `StatelessWidget` never changes; its appearance is entirely determined by the configuration it is given when initialized. A `StatefulWidget` is dynamic; it can change its appearance in response to events triggered by user interactions or when it receives new data.
  * *Link:* [Introduction to State Management](https://docs.flutter.dev/data-and-backend/state-mgmt/intro)

### Quiz Tasks
* **Task 4: Core Language (Single Choice)**
  * *Question:* Which programming language is primarily used to write Flutter applications?
    * [ ] Java
    * [ ] JavaScript
    * [x] Dart
    * [ ] Swift
  * *Customized Error Message:* Incorrect. While Java and Swift are used for native mobile development, Flutter uses Google's own programming language, which is Dart.
* **Task 5: Identifying Layouts (Multiple Choice)**
  * *Question:* Which of the following are considered layout widgets in Flutter? (Select all that apply)
    * [x] Column
    * [x] Row
    * [ ] Text
    * [x] Stack
  * *Customized Error Message:* Incorrect. `Text` is a structural UI element used to display strings, not a layout widget. Layout widgets like `Column`, `Row`, and `Stack` are specifically used to arrange other widgets on the screen.
* **Task 6: State Mutability (Single Choice)**
  * *Question:* Which method must be called to safely update the UI in a `StatefulWidget`?
    * [ ] `updateUI()`
    * [ ] `refresh()`
    * [x] `setState()`
    * [ ] `build()`
  * *Customized Error Message:* Incorrect. The `build()` method is called automatically by the framework. To trigger a rebuild and update the state manually, you must use the `setState()` method.

### Coding Tasks
* **Task 7: Hello World**
  * *Description:* Create a basic text element that displays "Hello World" on the screen.
  * *Placeholder Code:* `return ____('Hello World');`
  * *Expected Output:* `return Text('Hello World');`
* **Task 8: Building a Vertical Layout**
  * *Description:* Arrange two `Text` widgets vertically using a `Column` widget.
  * *Placeholder Code:*
    ```dart
    return ____(
      children: [
        Text('Item 1'),
        Text('Item 2'),
      ],
    );
    ```
  * *Expected Output:* `return Column(...)`
* **Task 9: Updating State**
  * *Description:* Inside the `incrementCounter` method of a StatefulWidget, properly update the `_counter` variable so the UI reflects the change on the screen.
  * *Placeholder Code:*
    ```dart
    void incrementCounter() {
      ____(() {
        _counter++;
      });
    }
    ```
  * *Expected Output:* `setState(() { _counter++; });`

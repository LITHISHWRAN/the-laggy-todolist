# Flutter Learning Journey

## 1. Stateless vs. Stateful Widgets
In Flutter, widgets are classified based on whether their configuration can change:
* **StatelessWidget:** These are immutable. Once they are built, their properties cannot change (e.g., an Icon, a Label, or a static logo). They are used for UI parts that just depend on configuration info.
* **StatefulWidget:** These maintain a mutable state that can change during the widget's lifetime. When the state changes (like a counter incrementing), the widget rebuilds to reflect the new data.

## 2. The Widget Tree & Reactive UI
Flutter builds UIs using a **Widget Tree**, which is a hierarchy of widget objects.
* **Composition:** Everything is a widget (padding, alignment, layout). We compose simple widgets to build complex layouts.
* **Reactivity:** When `setState()` is called, Flutter marks the widget as "dirty." It then efficiently checks the widget tree to see what has changed and only re-renders the necessary parts. This makes UI updates incredibly fast (60fps).

## 3. Why Dart?
Dart is the secret sauce behind Flutter's performance:
* **JIT (Just In Time) Compilation:** Allows for "Hot Reload" during development, letting you see code changes instantly without losing app state.
* **AOT (Ahead Of Time) Compilation:** Compiles to native ARM machine code for production, ensuring fast startup times and smooth performance.
* **Sound Null Safety:** Reduces runtime crashes by making null errors a thing of the past.

## 4. Project Demo
* **Project:** Counter App
* **Functionality:** A button press updates the on-screen counter instantly using Flutter's reactive state management.
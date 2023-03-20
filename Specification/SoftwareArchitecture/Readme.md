# Software Architecture isn't ready (Draft 3)

**Best practices in Flutter**:
Needed practices:
- Foldes structure
![image](https://user-images.githubusercontent.com/45210795/214284000-8eb1750b-e00f-4c49-b252-8fa102681989.png)
- BLoC
  - about https://www.mitrais.com/news-updates/getting-started-with-flutter-bloc-pattern/
  - how to start https://bloclibrary.dev/#/gettingstarted
  - examples with well-defined architecture with BLoC https://bloclibrary.dev/#/flutterlogintutorial
- DI in Flutter:
  - https://fluttergems.dev/state-management/
  - https://pub.dev/packages/get
  - https://pub.dev/packages/get_it
  - https://pub.dev/packages/injectable
  - https://pub.dev/packages/kiwi
  - https://pub.dev/packages/provider
  examples:
    - https://www.youtube.com/watch?v=KNcP8z0hWqs&ab_channel=ResoCoder
    - https://blog.logrocket.com/dependency-injection-flutter-using-getit-injectable/

Referecies:
- https://applover.com/blog/flutter-architecture-best-practices-for-your-mobile-projects/
- https://verygood.ventures/blog/very-good-flutter-architecture
- https://docs.flutter.dev/resources/architectural-overview
- https://viblo.asia/p/what-are-the-key-strategies-and-best-practices-that-simplify-flutter-app-development-3kY4gn2OVAe
- https://blog.logrocket.com/complete-guide-flutter-architecture/
- https://surf.dev/flutter-architecture-guide/
- https://codewithandrea.com/articles/flutter-repository-pattern/
- https://dev.to/noureldinshobier/building-scalable-flutter-apps-architecture-styling-conventions-state-management-40c9
- https://www.mobindustry.net/blog/how-to-implement-the-bloc-architecture-in-flutter-benefits-and-best-practices/
- https://radixweb.com/blog/overview-of-flutter-architecture
- https://cheesecakelabs.com/blog/architect-flutter-projects/
- https://dev.to/noureldinshobier/building-scalable-flutter-apps-architecture-styling-conventions-state-management-40c9
- https://www.altexsoft.com/blog/engineering/pros-and-cons-of-flutter-app-development/
- https://blog.back4app.com/flutter-alternatives/
- https://itnext.io/scalable-state-management-on-flutter-using-stacked-architecture-ac2a5d419eaa
- https://flutterawesome.com/a-modular-app-architecture-that-can-be-scalable-as-the-time-passes/
- https://verygood.ventures/blog/very-good-flutter-architecture
- https://medium.com/@sushaanshakya88/maintaining-scalable-architecture-in-flutter-6bc0524d3864
- https://aglowiditsolutions.com/blog/flutter-best-practices/#:~:text=BLoC%20Architecture%20is%20the%20best,Web%2C%20watchOS%2C%20and%20more.
- https://medium.com/@nikilapi/i-found-the-perfect-architecture-for-flutter-apps-59fc2dc8f00f
- https://stackoverflow.com/questions/63677649/flutter-best-architecture-patterns
- https://medium.flutterdevs.com/design-patterns-in-flutter-part-2-mvp-e17b3be2e51b
- https://medium.flutterdevs.com/design-patterns-in-flutter-part-2-mvp-e17b3be2e51b
- https://medium.flutterdevs.com/design-patterns-in-flutter-part-1-c32a3ddb00e2

<br>

<br>
<br>
<br>

**flutter communication with android service**:
- https://www.google.com/search?q=flutter+communication+with+android+service&oq=flutter+communication+with+android+service&aqs=chrome..69i57.14473j0j7&sourceid=chrome&ie=UTF-8
- https://medium.com/codechai/flutter-and-services-638ebfbbe47f
- https://docs.flutter.dev/development/packages-and-plugins/background-processes
- https://docs.flutter.dev/development/platform-integration/platform-channels
- https://docs.flutter.dev/get-started/flutter-for/android-devs
- https://dev.to/blazebrain/using-services-in-flutter-572h
- https://youtu.be/exHgLlF9XlQ
- https://learn.microsoft.com/en-us/answers/questions/772581/communication-services-for-flutter-apps.html
- https://betterprogramming.pub/how-does-flutter-communicate-with-platform-native-code-2bb002f64121
- https://medium.com/flutter-community/creating-services-to-do-the-work-in-your-flutter-app-93d6c4aa7697
- https://pusher.com/tutorials/how-to-add-realtime-communication-to-flutter-with-pusher-channels/
-  



SOLID:
https://youtube.com/playlist?list=PLmqFxxywkatQNWLG1IZYUhKoQrnuZHqaK


draw.io link:
https://app.diagrams.net/#G17zhYh2qk37QgLhyynme0vzYZO9Z538Fd


<br>
<br>
<br>
<br>
<br>

#### Scenarios
1. Developer story. [TODO: issue reference]()<br>
**On device button event scenario**.<br>
When **on device button event scenario** is launched - then the storage of the log should be updated,<br>
and if it is **Active state** of the app - then the view of the log should be updated regarding the **filter text input** content.<br>
2. User story. [TODO: issue reference]()<br>
**Clear log scenario**.<br>
As a user, I want to have an option to clear the log.<br>
When **clear log scenario** is launched - it opens the **clear log confirmation window**.<br>
4. User story. [TODO: issue reference]()<br>
**On filter text changed scenario**.<br>
5. Product Owner story. [TODO: issue reference]()<br>
**Show About scenario**.<br>
When **show About scenario** is launched - it **About app screen** opens.<br>
6. User story. [TODO: issue reference]()<br>
**Quit app scenario**.<br>
As a user, I want to have an option to quit tha app.<br>
When a **quit app scenario** is launched - then the app closes.<br>
<br>

#### Events
1. Developer story. [TODO: issue reference]()<br>
**On device button event**.<br>
When some device physical button was pressed - the **on device button event scenario** should be launched.
2. Developer story. [TODO: issue reference]()<br>
**On paused**.<br>
...
3. Developer story. [TODO: issue reference]()<br>
**On actived**.<br>
...
4. Developer story. [TODO: issue reference]()<br>
**On opened**.<br>
...
<br>

#### States
**Closed state** - the app is closed.<br>
**Active state** - the app is application visible on the screen.<br>
**Paused state** - the app is not in **active state** and not in **closed state**.<br>
1. Developer story. [TODO: issue reference]()<br>
**Closed state**.<br>
If the app is not running, there should be background process<br>
to be able to handle **on device button event**.
<br>
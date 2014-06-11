DiOS
====

DiOS is a practical system to perform automated dynamic privacy analysis of iOS apps. DiOS provides a highly scalable and fully automated solution to schedule apps from the official Apple App Store for privacy analysis to iOS devices. While apps are automatically executed, user interaction is simulated using random and smart execution strategies, and sensitive API calls as well as network connections are tracked.

DiOS allows for structured exploration and navigation of an app's UI by leveraging the automated
UI testing support provided by the official Apple development tools. Originally, this feature was intended to simplify UI tests during an app's development phase. However, we successfully reverse engineered the inner workings to retrofit even existing App Store apps to make use of Apple's [UI automation](http://developer.apple.com/library/ios/#documentation/DeveloperTools/Reference/UIAutomationRef/) features. This allowed us to investigate several robust UI exploration strategies that simulate user interaction and thus optimize an app's UI coverage.

One of the core features of DiOS is its pluggable architecture. While apps are automatically executed and user interaction is simulated using smart execution strategies, any analysis component can be integrated easily.

Basically, the DiOS system consists of three major parts: a [backend](https://github.com/DiOS-Analysis/Backend) that is mainly used as central data storage, a [worker](https://github.com/DiOS-Analysis/Worker) used as connecting link between the backend and any number of attached iOS devices, and several [client components](https://github.com/DiOS-Analysis/Pilot) running on the connected iOS devices. Each of these components will be explained in more detail within the appropriate repository.

* For general questions on DiOS, please contact us at dios@i1.cs.fau.de. For feature requests or bug reports, please use the issue tracking system: https://github.com/DiOS-Analysis/DiOS/issues.

* The [full report](http://opus4.kobv.de/opus4-fau/files/4755/report.pdf) as well as videos demonstrating DiOS in action are available from our project site: https://www1.cs.fau.de/dios/.

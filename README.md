DiOS: Dynamic Privacy Analysis of iOS Applications
==================================================

DiOS is a practical system to perform automated dynamic privacy analysis of iOS apps. DiOS provides a highly scalable and fully automated solution to schedule apps from the official Apple App Store for privacy analysis to iOS devices. While apps are automatically executed, user interaction is simulated using random and smart execution strategies, and sensitive API calls as well as network connections are tracked.

DiOS allows for structured exploration and navigation of an app's UI by leveraging the automated
UI testing support provided by the official Apple development tools. Originally, this feature was intended to simplify UI tests during an app's development phase. However, we successfully reverse engineered the inner workings to retrofit even existing App Store apps to make use of Apple's UI automation features. This allowed us to investigate several robust UI exploration strategies that simulate user interaction and thus optimize an app's UI coverage.

One of the core features of DiOS is its pluggable architecture. While apps are automatically executed and user interaction is simulated using smart execution strategies, any analysis component can be integrated easily.

The full report as well as videos demonstrating DiOS in action are available from our project site: [https://www1.cs.fau.de/dios/].

# Eclipse Platform

The Eclipse platform is structured around the concept of **plug-ins**. Plug-ins are structured bundles of code and/or data that contribute functionality to the system. Functionality can be contributed in the form of code libraries \(Java classes with public API\), platform **extensions**, or even documentation. Plug-ins can define **extension points**, well-defined places where other plug-ins can add functionality.

Each subsystem in the platform is itself structured as a set of plug-ins that implement some key function. Some plug-ins add visible features to the platform using the extension model. Others supply class libraries that can be used to implement system extensions.

The Eclipse SDK includes the basic platform plus two major tools that are useful for plug-in development.  The Java development tools \(JDT\) implement a full featured Java development environment.  The Plug-in Developer Environment \(PDE\) adds specialized tools that streamline the development of plug-ins and extensions.

These tools not only serve a useful purpose, but also provide a great example of how new tools can be added to the platform by building plug-ins that extend the system.

![](/assets/eclipse_platform.png)


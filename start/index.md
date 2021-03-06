---
layout: default
title: Getting started
published: true
---


<p class="text-center">
   <a class="btn" href="http://update.rascal-mpl.org/stable"><i class="icon-download-alt"></i> Eclipse update site</a>
   <a class="btn" href="http://update.rascal-mpl.org/console/rascal-shell-stable.jar"><i class="icon-download"></i> Commandline REPL Jar File</a>
</p>

## Disclaimer

We currently only release alpha versions of Rascal, which are subject to frequent changes

## Eclipse plugin

The Eclipse update site for Rascal is: **[http://update.rascal-mpl.org/stable/](http://update.rascal-mpl.org/stable/)**

You need _Eclipse for RCP Developers (Mars.1)_ version of Eclipse
available at [www.eclipse.org/downloads/](http://www.eclipse.org/downloads/) to run Rascal. 

Please note that:
 
 - Rascal needs a JDK because it uses the Java compiler, so please download a JDK8, not just a JRE.
 - You may have to [edit the Eclipse init file](/start/editini.html) so
   that Eclipse can find your Java installation and Eclipse can allocate enough
   resources. If you are running MacOSX you have to start Eclipse once first, quit, and then edit the ini file.
 - For generating parsers, Rascal uses quite a bit of memory. Please use `-vmargs -Xmx1G -Xss32m`
 
### Follow these steps to install the plugin into Eclipse

1. Start Eclipse.
1. Select Help -> Install New Software.
1. Make sure that the tick for "Contact all update sites during install to find required software" is enabled.
1. Type: `http://update.rascal-mpl.org/stable/` in the "Work with" edit box, and then press enter.
1. Select the feature *Rascal* (only the Rascal Metaprogramming Language is needed).
1. Select Next (several times) and accept the software license. The process may take a few minutes!
1. Once these features have been installed, restart Eclipse.
1. In case of problems check our [Troubleshooting page](http://www.rascal-mpl.org/help/troubleshooting.html)

### How to use the Eclipse plugin for the first time

After you have downloaded Rascal, you might be interested in the first steps to executing some Rascal code.

 - Open the Rascal Perspective (use the "Open Perspective" button in the top-right of your screen)
 - Create a new Rascal project (use the "New..." button in the top-left of your screen, then select "Rascal Project" from the menu)
 - This should automatically open a new console with the new project on its search path
 - Type `1 + 1` after the `rascal>` prompt to see `2`

## Commandline REPL

An entirely different way of using Rascal is via the standalone commandline console.
You can download the fully contained jar file [here](http://update.rascal-mpl.org/console/rascal-shell-stable.jar).

Please note that:

- The commandline version does not support analyzing Java code directly at the moment.
- A Java JDK 1.8 or higher installed is required. A Java run-time environment (JRE) will not be enough.
- The command line of Rascal starts by running `java -Xmx1G -Xss32m -jar rascal-<version>.jar`.

## Further reading

Check out our [Help page](/help/) for links to documentation and our community.

---
layout: page
title: "Installation & setup"
category: doc
date: 2014-11-14 12:00:00
---

#Installation and setup

All components are available as both NuGet packages and MSI installers.


##NuGet
The NuGet packages are intended to be used to reference the components from Visual Studio when creating a pipeline.

Note that NuGet won't copy the component to BizTalk's pipeline components folder so it won't automatically show up in the pipeline component toolbox in Visual Studio.
For that to happen you must either manually copy it to the PipelineComponents folder in the BizTalk installation directory or explicitly point Visual Studio to it in the _Choose toolbox items_ menu.

After you have referenced the NuGet package from a BizTalk pipeline project do the following to add it to the toolbox:

1. In the pipeline designer windows in Visual Studio right click the toolbox on the left hand side and choose _Choose Items_
2. Select the _BizTalk Pipeline Components_ tag.
3. Press the _Browse_ button.
4. Browse to your project directory and locate the component assembly in the packages folder.
5. Press open to close the dialog.
6. Make sure that the components is checked.
7. Press OK to close the dialog and add the component to your toolbox.

##MSI
The MSI's are intended for deploying the component to your BizTalk environment. 
Just run the installer to add the component to the GAC.
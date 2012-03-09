#Plugins and Packages

##What is a plugin?
A Plugin is a single component of functionality that extends the back-office; these include a Tree, an Editor or a Property Editor, to name a few.

##What is a package?
A Package is a collection of Plugins that have been prepared for installation into the back-office.

##Types of plugins
The following types of plugin can extend the back-office.

###[Applications](Applications.md)
An application defines a section of the back-office. A default Umbraco installation comes with several default applications - these are Content, Media, Settings, etc.

###[Trees](Trees.md)
Trees are building blocks of application sections. An application contains one or more Trees, for example the Settings section consists of several trees; e.g. the Stylesheet tree, the Document Types tree, etc.  Each Tree can contain nodes, with each node providing specific functionality.

###[Menu Items](MenuItems.md)
Trees (and nodes within a Tree) can have additional functionality via its (right-click) context menu. These menu items perform custom actions for the selected item.

###[Editors](Editors.md)
An Editor enables interactions in the right/main editor panel and modal dialogs in the back-office. Typically these are used for editing content, scripts or templates.

###[Dashboards](Dashboards.md)
A Dashboard provides a piece of functionality to enhance an application section. These usually appear as the default panel within a section.

###[Macros](Macros.md)
A Macro is a contained piece of functionality, generally used on the front-end of a website.

###[Property Editors](PropertyEditors.md)
A Property Editor offers functionality that can be used by a content editor to input data. Interaction with a Property Editor is achieved by referencing it with a [Data Type](null).

###[Parameter Editors](ParameterEditors.md)
A Parameter Editor is similar to a Property Editor in that they are used to capture input data; however the purpose of a Parameter Editor is to be used exclusively on Macros.

***

##Package format
The format used for packages follows the [NuGet](http://nuget.org) specification. For more information about the NuGet specification, please visit the [NuGet Documentation](http://docs.nuget.org) website. Further details of how to create NuGet packages for Umbraco are outlined [here](#TBC).

##How are packages installed?
When a package is uploaded, ready to be installed, it will be stored in the `\App_Data\Umbraco\LocalPackages` folder. Once installed the package contents are installed in the `\App_Plugins\Packages` folder.
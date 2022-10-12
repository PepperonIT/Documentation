# Tools/technologies
## tl;dr 
The documentation should start with a tl;dr about what the tools do and why they were chosen. If there is a critical functionality being provided by the tool it should be specified what it is and where it is needed. It should generally be done as shown below.

```
Tool 1
```
Tool 1 was chosen because it is important for this functionality, it also has pre-built interoperability with this other thing, which is useful since we use that as well. If another alternative was considered it can be mentioned here, that way it is easy to find if problems arise from this tool later on and it has to be removed from the project. If applicable, a link to the tools own documentation or website/github should be provided *here*.

```
Tool 2
```
Tool 2 was chosen... etc.

```
Tool 3 
```
Tool 3 was chose... etc.

# Installation of tool x
In this section the installation and set up process for each tool should be documented, for all relevant operating systems. If the tool is not available for a specific operating system or if it is mainly supported for a specific operating system this should be mentioned here. 

## Linux/Debian
Begin by defining prerequisit installations and how to install them, this should obviously be done in order of dependencies. That is, if we require both tools Y, and Z for tool X to function but Y also require Z. Then we begin by documenting the install process for tool Z.

If there exists a installation guide that was used it should be referenced here, *note that it is not enough to just provide a link to an existing guide*. We can not guarantee that the guide will remain available and installation tutorials usually don't follow a standard. This can make it difficult to go back and find a specific step in the installation process later. 

A tutorial for the installation of Z can be found [here](https://github.com/incognite-lab/Pepper-Controller).

Begin by providing a way to check which version of the tool is installed or if it is installed at all at the beginning of the process. These steps can usually be combined since a version check will fail if the tool is not installed.
```
Run this command to check if the tool is installed
```
We expect it to return this output:
```
If applicable format the expected output here
Or if not applicable describe the expected outcome
```

Beneath this there should be a way to completely uninstall the tool from the system. It may seem strange to have this in the installation documentation, but it can be very useful if the wrong version is installed or otherwise corrupted. 
```
Uninstall command
```

This should then be followed by the installation process, step-by-step, and with verification steps as needed. These verifications can be things such as "run this to see that it has been extracted to the correct folder", or "run this command to check the version which also verifies that it is installed". All manual input by the user should be clearly indicated.
```
Like this
```
This makes it easy to find the key points in the documentation, since only user input and expected output will be contained in these fields.

At the end of the installation process there *must* be a concise way to verify that the installation was completed successfully. If there is no clear way to verify the installation make one. This can be done several ways, for instance by creating scripts that does it for the user or running a "dummy program". The dummy program can be something as simple as importing the package, if it is installed correctly it should compile and run. For more complex tools links to resources should be added here as well, this can either link to tutorials or official documentation. If a uninstall process was not previously provided it should be provided here.



## Windows
...
## etc
...

# Tool W
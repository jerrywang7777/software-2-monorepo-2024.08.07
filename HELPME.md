# Troubleshooting Guide

You may run into a variety of problems while using VSCode to run Java code.
I will document as many of the problems as we've run into here, so you can
browse them.

## Unit Testing Is Not Working

Sometimes you might run into an issue where unit testing is not working.
One possible solution is to clean the workspace by clicking on the
three dots next to the Java Projects tab in the Explorer window and select
"Clean Workspace". You may also be able to replicate this by searching
for "Clean Workspace" in the command palette (i.e., `CTRL + SHIFT + P`).

If cleaning the workspace does not work, there may be alternative problems.
For example, VSCode and Java have a nasty bug where file paths that include
special characters, such as characters from other languages like Chinese or
Hebrew, cause unit testing to fail. See
[this thread](https://github.com/microsoft/vscode-java-test/issues/1159)
for discussion around the issue. The short term solution is to move the repo to
a folder without special characters in the path.

# Terminal Tab Is Missing in VSCode

Sometimes you will go looking for a tab at the top of the VSCode window, and
it will appear to be missing. No worries, it's probably hidden in the `...`
menu. Click that and you should see the terminal tab as well as anything else
that might be missing.

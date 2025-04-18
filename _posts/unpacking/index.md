---
title: "Simple UPX unpacking (MinGW)"
classes: wide
header:
  teaser: /assets/images/CTF/0xL4ugh/path.png
ribbon: DodgerBlue
description: "Simple tutorial on how to debug and unpack packed executables."
categories:
  - Unpacking
toc: true
---

# Unpacking

# String modification

Today, we'll explore how to modify the strings (text) of executable files. When we run an executable file, strings like "Hello World!" that appear on the GUI are usually located in the `.rdata` or `data` segments. These are parts of the PE file structure used by the program to hold constant values like string literals.

Below is an example of these data segments shown in the program CFF Explorer, for an example crackme `LSDtrip.exe`:

![error loading](/assets/images/CTF/0xL4ugh/org.png)

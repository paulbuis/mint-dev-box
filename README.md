# Packer template for Mint Cinnamon 

Fork of [r-a-p-a/mint-dev-box](https://github.com/r-a-p-a/mint-dev-box)

Not aiming at professional developers in Great Britain.

Aiming at Ball State University Computer Science undergraduates in Programming Languages Course I teach.

##Goals:
* Convert to US locale / keyboard layout / Eastern Time Zone
* Drop RAM requirement from 6GB to 3GB for student rather than developer machines
* Try for 32-bit OS rather than 64 bit OS for students having problems enabling virtualization in BIOS
* Update to Node 6.x rather than deprecated Node 5.x
* Update to Swift 3.0 (Preview-2) from Swift 2.x
* Add C# and F# packages
* Add Java 9 (keep Java 8) for jshell REPL
* Add Packer so I can host this project in a Mint box rather than a Windows box
* Include support for Mint Cinnamon 18.x

###Goals that maybe should be moved to later Vagrant provisioning stage
* Include additional Go tools: golint, godep (needed by Microsoft Visual Studio Code editor)
* Add additional vagrant guest to host directory mapping(s)

##Anticiapated Challenges
* Swift distro currently has CoreFoundations directory not world readable, need to add step to recursively chmod a directory

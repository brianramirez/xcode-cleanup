# Xcode Cleanup

Xcode makes a mess sometimes, this simple utility will help clean it up.

## Purpose

This is a simple command line utility that was written to be a cron job on a Jenkins build machine.

 It completely "cleans" (a.k.a. deletes) the following locations on your Mac so be careful!

- `~/Library/Developer/Xcode/Archives`
- `~/Library/Developer/Xcode/DerivedData`

### Installation & Usage

#### From Source

1. Open the Xcode project.
1. Choose your code signing option (if required)
1. Select Product > Archive from the Finder menu bar.
1. Once Archiving finishes the Organizer should open, if it does not, open it by selecting Window > Organizer
1. Select `xcode-cleanup` from under the "Other Items" section on the left side of the Organizer
1. Choose Export
1. Select Built Products and choose where you want to save the executable.
1. Copy the `xcode-cleanup` file to `/usr/local/bin` so it can easily be used from the Terminal

#### From Archive

1. Unzip the utility.
1. Copy the `xcode-cleanup` executable to `/usr/local/bin`

#### Using

1. Open a Terminal
1. Type `xcode-cleanup` and hit return
1. That's it!

## Goals

This is an extremely simple utility so it doesn't have a large roadmap, execpt possibly bundling it with other tools with a UI.

If you have ideas, suggestions, feel free to open a Pull Request.

## License

This utility is released under the [MIT License](LICENSE.md).

After some poking around in Xcode’s package contents, I found a way to edit all the if, switch, class, methods etc. snippets to have the opening curly brace on its own line. This is our convention, and I bet we’re not alone. Adding a manual new line for every `if` statement is waste of good brain power, so why not let Xcode do it right in the first place?

If your convention is something else, keep using it. If you’re cool, and want your if statements like this:

    if (YES)
    {
        NSLog(@"Tidy code == win!");
    }

Then:

* Run the script [here][gisturl] whenever you update Xcode, and you’ll always have the latest version of this snippet fix.

> **Note:** the linked script always checks out the latest version. If you’re using it with an older version of Xcode, you’ll want to modify the script to get the appropriate version of the code snippet. Homework for someone: make the script get the right version of the snippets file for every version of Xcode it might encounter. I recommend a mapping table of Xcode versions to hashes of commits in this repo.

[gisturl]: https://gist.github.com/ZevEisenberg/5167026

Or, if you want to install it manually:

* Quit Xcode

* Make a backup of

	Xcode 4.2.x: `/Developer/Library/Xcode/PrivatePlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`

	Xcode 4.3+: `/Applications/Xcode.app/Contents/PlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`

    Xcode 5.1+: `/Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Versions/A/Resources/SystemCodeSnippets.codesnippets`

* Make another backup if you intend to screw something up

* Download the linked file to your desktop as `SystemCodeSnippets.codesnippets`

* Copy your desktop’s `SystemCodeSnippets.codesnippets` to

	Xcode 4.2.x: `/Developer/Library/Xcode/PrivatePlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`

	Xcode 4.3+: `/Applications/Xcode.app/Contents/PlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`

    Xcode 5.1+: `/Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Versions/A/Resources/SystemCodeSnippets.codesnippets`

* Start Xcode

Then:

* Type wonderful `if`, `else`, `switch` and `for` statements all day long!

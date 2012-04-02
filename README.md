After some poking around in Xcode 4.2's files, I finally found a way to edit all the if, switch, class, methods etc. snippets to have the opening curly brace on its own line. This is our convention, and I bet we're not alone. Adding a manual new line for every `if` statement is waste of good brain power, so why not let Xcode do it right in the first place?

If your convention is something else, keep using it. If you're cool, and want your if statements like this:

    if (YES)
    {
        NSLog(@"Tidy code == win!");
    }

Then:

* Quit Xcode

* Make a backup of
	
	Xcode 4.2.x: `/Developer/Library/Xcode/PrivatePlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`
	
	Xcode 4.3.x: `/Applications/Xcode.app/Contents/PlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`

* Make another backup if you intend to screw something up

* Create a file on your desktop called: `SystemCodeSnippets.codesnippets`

* Download the linked file to your desktop

* Copy your desktop's `SystemCodeSnippets.codesnippets` to

	Xcode 4.2.x: `/Developer/Library/Xcode/PrivatePlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`
	
	Xcode 4.3.x: `/Applications/Xcode.app/Contents/PlugIns/IDECodeSnippetLibrary.ideplugin/Contents/Resources/SystemCodeSnippets.codesnippets`


* Start Xcode

* Type wonderful `if`, `else`, `switch` and `for` statements all day long!

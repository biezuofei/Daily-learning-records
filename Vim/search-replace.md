# vim --search and replace

The vim can hit shit : and hit %s///g . Give it a try.

:s/foo/bar/g 	Change each 'foo' to 'bar' in the current line.
:%s/foo/bar/g 	Change each 'foo' to 'bar' in all the lines. 

```bash
$ vim --bar
```

See `man vim` for more details.
#	Search and replace in multiple buffers
	Often search and replace is needed in multiple files. 
	This tip uses the procedures from run a command in multiple buffers 
	to show how a substitute may be executed multiple times 
	using :argdo (all files in argument list), 
	or :bufdo (all buffers), 
	or :tabdo (all tabs), 
	:windo (all windows in the current tab), 
	or :cdo (all files listed in the quickfix list). 
	All buffers
	:bufdo %s/pattern/replace/ge | update
	All windows
	:sball
	<C-w>
	:windo %s/pattern/replace/ge 	Search and replace in all visible windows.
	 All files in a tree
	:arg *.cpp 	All *.cpp files in current directory.
	:argadd *.h 	And all *.h files.
	:arg 	Optional: Display the current arglist.
	:argdo %s/pattern/replace/ge | update 	Search and replace in all files in arglist
	:arg **/*.cpp 	All *.cpp files in and below current directory.
	:argadd **/*.h 	And all *.h files
	


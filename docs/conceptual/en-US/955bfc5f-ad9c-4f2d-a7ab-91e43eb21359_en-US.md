# List.sortBy<'T,'Key> Function (F#)

Sorts the given list using keys given by the given projection. Keys are compared using [Operators.compare](http://msdn.microsoft.com/en-us/library/295e1320-0955-4c3d-ac31-288fa80a658c).

**Namespace/Module Path:** Microsoft.FSharp.Collections.List

**Assembly:** FSharp.Core (in FSharp.Core.dll)


## CAPS_SYNTAX_MD

```
// Signature:
List.sortBy : ('T -> 'Key) -> 'T list -> 'T list (requires comparison)

// Usage:
List.sortBy projection list
```

#### CAPS_PARAMETERS_MD
*projection*
Type: **'T -&gt; 'Key**


The function to transform the list elements into the type to be compared.


*list*
Type: **'T**[list](http://msdn.microsoft.com/en-us/library/c627b668-477b-4409-91ed-06d7f1b3e4a7)


The input list.



**The sorted list.**
## CAPS_REMARKS_MD
This is a stable sort, that is, the original order of equal elements is preserved.

This function is named **SortBy** in compiled assemblies. If you are accessing the function from a language other than F#, or through reflection, use this name.

**The following code example illustrates the use of List.sortBy.**
**[!CODE [FsLists#6](../CodeSnippet/VS_Snippets_Fsharp/fslists/FSharp/fs/program.fs#6)]**
**Output**
**[1; -2; 4; 5; 8]**
## Platforms
Windows 8, Windows 7, Windows Server 2012, Windows Server 2008 R2


## Version Information
**F# Core Library Versions**

Supported in: 2.0, 4.0, Portable




## See Also
[Collections.List Module &#40;F&#35;&#41;](Collections.List+Module+%28F%23%29.md)

[Microsoft.FSharp.Collections Namespace &#40;F&#35;&#41;](Microsoft.FSharp.Collections+Namespace+%28F%23%29.md)

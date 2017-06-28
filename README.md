# Markdown-HOWTO

[Github Markdown Cheet Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
[Github Markdown Doc](https://help.github.com/categories/writing-on-github/)
[John Gruber's Original Markdown Spec](https://daringfireball.net/projects/markdown/)

## My Examples
### Table
#### Markdown Table
`<br>` insert line break.
```markdown
Shortcut | Description
---------|------------
`CTRL+SHIFT+p` + `menu` <br> or `ALT`|Toggle menu bar
```
#### HTML Table
Use `<pre lang=''>` for syntax highlighting in HTML table (see [StackOverflow Answer](https://stackoverflow.com/questions/21878143/github-markdown-syntax-highlight-of-code-blocks-in-the-table-cell)).
```html
<table><tr>
<td>
   <pre lang="csharp">
   const int x = 3;
   const string y = "foo";
   readonly Object obj = getObject();
   </pre>
</td>
<td>
  <pre lang="python">
  import matplotlib.pyplot as plt
  </pre>
</td>
<td>
  Variables defined with <code>def</code> cannot be changed once defined. This is similar to <code>readonly</code> or <code>const</code> in C# or <code>final</code> in Java. Most variables in Nemerle aren't explicitly typed like this.
</td>
</tr></table>
```
<table><tr>
<td>
   <pre lang="csharp">
   const int x = 3;
   const string y = "foo";
   readonly Object obj = getObject();
   </pre>
</td>
<td>
   <pre lang="python">
   import matplotlib.pyplot as plt
   </pre>
</td>
<td>
  Variables defined with <code>def</code> cannot be changed once defined. This is similar to <code>readonly</code> or <code>const</code> in C# or <code>final</code> in Java. Most variables in Nemerle aren't explicitly typed like this.
</td>
</tr></table>

### Image vs. Clickable Image
Pure markdown image can not size image, but HTML anchor `<a>` can. See
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#youtube-videos

```markdown
# Define a Reference Link
[CMake Logo]: https://cmake.org/wp-content/uploads/2014/06/cmake_logo-main.png

# Non-clickable Image
![CMake][CMake Logo]

# Clickable Image
[![alt][CMake Logo]](http://cmake.org)
```
[CMake Logo]: https://cmake.org/wp-content/uploads/2014/06/cmake_logo-main.png

![CMake][CMake Logo]

[![alt][CMake Logo]](http://cmake.org)

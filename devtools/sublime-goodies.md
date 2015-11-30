## Sublime goodies for Front-end Developers

Introducing **Sublime Text 3** tips and goodies which always help me to write
code in very comfortable workspace.

===

#### Exclude node_modules out of Sublime Text 3 searches:
It will skip searching files from folders from the following array (works for `CMD`+`t` as well)

    "folder_exclude_patterns": [
      ".git",
      "node_modules",
      "bower_components",
      "dest",
      "build",
      "docs"
    ]

===

#### Remove extra whitespaces on save:
Keep it clean!

    "trim_trailing_white_space_on_save": true

===

#### Let it scroll more after the ending line:
Gives a screen sized extra scrollable area which is kinda cool

    "scroll_past_end": true

===

#### Use snippets for writting shortcuts:
For writting `console.log()` with `con` + `TAB`.

Open up your `Sublime Text 3` > `Tools` > `New Snippet`. Put this code there
and save the file in the given directory by default:

    <snippet>
        <content><![CDATA[console.log($1)$0]]></content>
        <tabTrigger>con</tabTrigger>
        <tabTrigger>log</tabTrigger>
        <scope>text.html,source.js</scope>
        <description>console.log()</description>
    </snippet>

Continue adding by your own.

===

#### Use Sublime Plugins
I've created a list of plugins, which I use frequently. I had created the
repository [Custom-Sublime-Look](https://github.com/nikoloza/Custom-Sublime-Look) earlier, but
now I'm gonna put it updated right here:

##### Recommended packages:

Syntax highlighs:
* [HTML5](https://sublime.wbond.net/packages/HTML5)
* [CSS3](https://sublime.wbond.net/browse/authors/y0ssar1an)
* [Less](https://sublime.wbond.net/packages/LESS)
* [Jade](https://sublime.wbond.net/packages/Jade)
* [SASS](https://sublime.wbond.net/packages/Sass)
* [SCSS](https://sublime.wbond.net/packages/SCSS)
* [Babel Sublime](https://github.com/babel/babel-sublime) - ES6 Syntax highlight

Must have tools:
* [HTML-CSS-JS Prettify](https://sublime.wbond.net/packages/HTML-CSS-JS%20Prettify)
* [Emmet](https://sublime.wbond.net/packages/Emmet)
* [SideBarEnhancements](https://sublime.wbond.net/packages/SideBarEnhancements)

Another great tools you can have:
* [JSHint Gutter](https://packagecontrol.io/packages/JSHint%20Gutter)
* [GitGutter](https://sublime.wbond.net/packages/GitGutter)
* [Alignment](https://sublime.wbond.net/packages/Alignment)
* [AutoPrefixer](https://github.com/sindresorhus/sublime-autoprefixer)
* [ColorPicker](https://sublime.wbond.net/packages/ColorPicker)
* [Markdown Preview](https://sublime.wbond.net/packages/Markdown%20Preview)

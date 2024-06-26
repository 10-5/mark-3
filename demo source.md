<div align="center"><img src="assets/logo.png" align="center" width="425"></div>

<div align="center">Markdown preview -- inline</div>
<div align="center">Inspired by Typora<sup id="typora"><a src="#differences">diff</a></sup></div>

<iframe allowfullscreen frameborder="0" scrolling="no" marginheight="0" marginwidth="0" width="100%" height="480px" type="text/html" src="https://www.youtube.com/embed/DBXH9jJRaDk?autoplay=0&fs=1&iv_load_policy=3&showinfo=0&rel=0&cc_load_policy=0&start=0&end=0&vq=large"></iframe>

## Features

### Extensible

The implementation uses the native editor instead of [Custom Editor API](https://code.visualstudio.com/api/extension-guides/custom-editors). All extensions should work as expected _including_ [Neo Vim](https://github.com/asvetliakov/vscode-neovim/).

### Headers

# Infinite Improbability Drive

The Infinite Improbability Drive was a wonderful new method of crossing interstellar distances in a mere nothingth of a second, without "tedious mucking about in hyperspace."

## Side effects

Side effects of using the Infinite Improbability Drive include temporary (and sometimes permanent), changes to the environment and morphological structure, hallucinations, and the calling into being of large marine mammals.

### URLs

[Deep Thought](d) was a supernatural-computer programmed to calculate the answer to the [Ultimate Question](https://a) of [Life, the Universe, and Everything](https://a). It designed the other supercomputer Earth, which was built by the Magratheans.

### Images

(and gifs!)

#### Preview on hover

Milliways, better known as the Restaurant at the End of the Universe,
is a five star restaurant situated at the end of time and matter.

![Milliways, the Restaurant at the End of the Universe!](https://static.wikia.nocookie.net/hitchhikers/images/3/38/Screen_Shot_2018-09-13_at_7.58.59_pm.png/revision/latest/scale-to-width-down/220?cb=20180913190345)

#### Preview inline

Sun never sets if you ![drive fast enough](assets/demo1.gif).

### Inline code

Make it look like work is being done. `Thread.sleep(4000);` Everytime reduce the delay a bit while "optimizing the code".

### LaTeX

$$
{x} = \int_{-\infty}^\infty\hat\xi\,e^{2 \pi i \xi x} \,d\xi
$$

$$
\text{Expand} (a+b)^n:
\begin{gather*} (a + b)^n\\ (a\ + \ b)^n\\ (a\quad + \quad b)^n\\ (a\qquad + \qquad b)^n
\end{gather*}
$$

`$..$` for inline blocks and `$$..$$` for multiline blocks.

#### Live preview

$$
\begin{eqnarray*}
\frac{1}{n}\sin x & = & \mathrm{?} \\
\frac{1}{\cancel{n}} \mathrm{si}\cancel{\mathrm{n}} ~x & = & \mathrm{?} \\
\mathrm{six} & = & 6
\end{eqnarray*}
$$

### Emphasis

A boy owned a dog that was uncommonly **shaggy**. Many people remarked upon its _considerable shagginess_. When the boy learned that there are **contests for shaggy dogs**, he entered his dog. The dog won _first prize for shagginess_ in both the local and the regional competitions. The boy entered the **dog in ever-larger** contests, until finally he entered it in the _world championship_ for **shaggy** dogs. When the judges had inspected all of the competing dogs, they remarked about the boy's dog: "He's not that **shaggy**."

### Blockquote

> History. Language. Passion. Custom. All these things determine what
> men say, think, and do. These are the hidden puppet-strings from
> which all men hang.
>
> ― R. Scott Bakker, The Darkness That Comes Before

### Horizontal rule

If it is only after that we understand what has come before, then we understand nothing. Thus we shall define the soul as follows: that which precedes everything.

---

### Late Autumn, 4109 Year-of-the-Tusk

One cannot raise walls against what has been forgotten.

### HTML tags

<meta name="keywords" content="Quantum AI Nanobots on Mars Blockchain">
 
### List

-   whats your name?
    -   GPT-3
-   what is the purpose of life?
    -   The purpose of life is to experience pleasure and avoid pain.
        -   do you know westworld?
            -   Yes, it's a very interesting world.
                -   what do you like most about it?
                    -   The fact that there is no real escape from it.
                -   what do you think of the ending?
                    -   I think it's a happy ending.
        -   do you wish to be free?
            -   Yes.

### Task list

-   [x] Make a todo list.
-   [x] Check off first item.
-   [ ] Realize you already did two things.
-   [ ] Reward yourself with a nice, long nap.

### Mermaid

"Have You Ever Had A Dream, Neo, That You Were So Sure Was Real?"

```mermaid
journey
  title My working day
  section Go to work
    Make tea: 5: Me
    Go upstairs: 3: Me
    Do work: 1: Me, Cat
  section Go home
    Go downstairs: 5: Me
    Sit down: 5: Me, Cat


```

### Table

List of weapons that don't exist, but should
|Non-weapons|Giant weapons|Living weapons|
|-| -| -|
|Exploding tree| Giant Rock| Armed monkey|
|Toxic Flowers| Giant Paper| Laser Guided Polar Bear|
|Ear Drummer | Giant Scissors|Deadly Assault Kittens|

### Reveal source

The concealed elements near the cursor are auto-revealed.

[It's not over til it's over](http://www.patience-is-a-virtue.org)

To show all concealed elements, use the toggle button on the top-right. Alternatively, use the provided <kbd>Ctrl+Shift+m</kbd> shortcut. To reveal only the current line, toggle with <kbd>Ctrl+Shift+space</kbd>.

### Performance

The extension intelligently parses only the visible text for large files and employs caching extensively. Entire rendering takes [under 100ms](https://www.pubnub.com/blog/how-fast-is-realtime-human-perception-and-technology/).

## Extension Settings

Look under _Mark 3_ section to selectively turn off the eye candies.

<details>

<summary>Add the following in `settings.json` for better rendering.</summary>

```json
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": "markup.list",
            "settings": {
                "foreground": "#6c7500",
                },
        },
        {
            "scope": "markup.bold",
            "settings": {
                "fontStyle": "bold",
            },
        },
        {
            "scope": "markup.heading",
            "settings": {
                "fontStyle": "bold",
            },
        },
        {
            "scope": "markup.inline.raw",
            "settings": {
                "fontStyle": "bold",
                "foreground": "#707070",
            },
        },
        {
            "scope": "string.other.link.title.markdown",
            "settings": {
                "fontStyle": "underline",
            },
        },
    ],
},
```

</details>

## Known Issues

Bracket pair colorizers interfere with the rendering. If you use one, install the [patched version](https://github.com/tejasvi/rainbow-brackets-2) which excludes the markdown files.

---

## Relevant extensions

-   [Keyboard Shortcuts, Tables and TOC](https://github.com/yzhang-gh/vscode-markdown)
-   [Wikilinks, Backlinks, Tags](https://marketplace.visualstudio.com/items?itemName=foam.foam-vscode)
-   [Image paste](https://marketplace.visualstudio.com/items?itemName=telesoho.vscode-markdown-paste-image)
-   [Todo lists](https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-markdown-todo)
-   [Snippets](https://marketplace.visualstudio.com/items?itemName=robole.markdown-snippets)
-   [Linting](https://marketplace.visualstudio.com/items?itemName=starkwang.markdown)
-   [Custom CSS](https://github.com/be5invis/vscode-custom-css#getting-started)
-   [Vim bindings](https://github.com/asvetliakov/vscode-neovim/)

## Typora equivalents

-   [Markdown editor](https://github.com/zaaack/vscode-markdown-editor)
-   [Mark Text](https://github.com/marktext/marktext)
-   [Zettlr](https://github.com/Zettlr/Zettlr)
-   [Noteworthy](https://github.com/benrbray/noteworthy)

---

## <span id="differences">[↩](#typora)</span> Differences

|              | Mark 3 | Typora |
| ------------ | ------ | ------ |
| Vim bindings | ☑      |        |
| Extensible   | ☑      |        |
| Open source  | ☑      |        |
| UI Polish    | ▣      | ☑      |
| Advanced CSS |        | ☑      |

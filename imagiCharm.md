## Welcome to the imagiCharm World! 

### Lesson 1: 

Pixels labelled by row first, then column, e.g. to turn the pixel of row 2 and column 4 on you enter: 
```markdown
m[2][4]=on 
```

Instead of just turning on the pixel, you can assign it a specific colour. The following will turn the pixel red (R). 
```markdown
m[2][4]=R
```

If you want to go a step further, you can specify an RGB (red-green-blue) colour. The colour is assigned by given each of the three colours an intensity value between 0 and 255. So red would be purely red, i.e. the values for green and blue would be 0: (255, 0, 0). 

```markdown
m[2][4]= (255, 0, 0) 
```

You can set a blink rate for the pattern drawn. The chosen pixel will now blink twice a second. 
```markdown
m[2][4]= (255, 0, 0) 
blinkrate = 2 
```

## Lesson 2: 

When you need to repeat parts of your code it is best to use functions. The syntax of functions looks like this (example from https://edu.imagilabs.com/)
```markdown
def apple():
  apple_color = (222, 96, 42)
  m[0][5] = apple_color
  m[1][4] = apple_color
  m[2][2] = apple_color
  m[2][3] = apple_color
  m[2][4] = apple_color
  m[2][5] = apple_color
  m[2][6] = apple_color
  m[3][1] = apple_color
  m[4][1] = apple_color
  m[5][1] = apple_color
  m[6][1] = apple_color
  m[7][2] = apple_color
  m[7][3] = apple_color
  m[7][4] = apple_color
  m[7][5] = apple_color
  m[7][6] = apple_color
  m[6][7] = apple_color
  m[5][7] = apple_color
  m[4][7] = apple_color
  m[3][7] = apple_color

apple()

```

Alternatively, you can also hand over a parameters in the brackets, e.g. by using RGB values handed over as a tuple: 

```markdown
def apple(apple_color):
  m[0][5] = apple_color
  m[1][4] = apple_color
  m[2][2] = apple_color
  m[2][3] = apple_color
  m[2][4] = apple_color
  m[2][5] = apple_color
  m[2][6] = apple_color
  m[3][1] = apple_color
  m[4][1] = apple_color
  m[5][1] = apple_color
  m[6][1] = apple_color
  m[7][2] = apple_color
  m[7][3] = apple_color
  m[7][4] = apple_color
  m[7][5] = apple_color
  m[7][6] = apple_color
  m[6][7] = apple_color
  m[5][7] = apple_color
  m[4][7] = apple_color
  m[3][7] = apple_color

apple((222, 96, 42))
```

The background colour can be changed using the background function. To set it to green, one would enter: 
```
background(G)
```

Characters can be displayed using the character function: 
To display the letter A one would enter: 
```
character('A')
```

The colour of the letter can be set using a second parameter handed over to the character function, and the background can be specified with a third parameter. A green A on a red background would be written as: 
```
character('A', G, R)
```


You can use the [editor on GitHub](https://github.com/PyKoch/PyKoch.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).


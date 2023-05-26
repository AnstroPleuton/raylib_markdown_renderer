# Raylib Markdown Renderer
Render text with markdown format using raylib!

## Warning!
This markdown is designed for **my specific uses**, feel free to contribute any changes you make with it!

## Features
It can render
- Header (with 6 different sizes)
- Horizontal rule
- Quoted text (may render them where it's unintended)
- Bold text
- Italic text
- Underscore (doesn't follow actual markdown format)
- Strike through
- Monospace inline code text
- Monospace code block
- Filled bullet points
- Hollow bullet points
- Ability to use escape codes to skip formatting

## Customization
You can customize the render by
- Font
  - Font size for main text
  - Font size for different headers
- Colors
  - Text color (limited, uses same color for all the text)
  - Monospace code background color
  - "Shape color" for horizontal rule, quote block and bullets

---
## Usage
Call the function DrawTextMarkdown. That's it!
```c
// Draw text with markdown formats (only basics)
void DrawTextMarkdown(FontCollection *fontCollection, const char *text, Rectangle area, float fontSizes[MARKDOWN_HEADER_SIZE_MAX], Vector2 spacing, float tabWidth, ColorCollection *colorCollection)
```
All the fonts that may be used by renderer are stored in one structure called `FontCollection`, make one and pass it as pointer :)
Same goes for all the colors as `ColorCollection` (~~CC~~), make one and pass it as pointer too!

## License
This project is licensed under MIT Licese, see [LICENSE](LICENSE).
The fonts (Roboto, RobotoMono) is licensed under [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0), see [LICENSE](LICENSE).

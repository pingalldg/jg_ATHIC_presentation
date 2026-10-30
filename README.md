[themes]: https://revealjs.com/themes
[config]: https://revealjs.com/config
[pandoc]: https://pandoc.org/

# Presentation template 

Template for making a presentation with markdown  
**Requires** the document converter [Pandoc][pandoc]

## Compiling with Pandoc
Pandoc is used to compile from Markdown to HTML. In a terminal, issue the command

    pandoc \
    -t revealjs \
    presentation.md \
    --standalone \
    -o presentation.html \
    -V theme=$theme \
    -V transition=convex \
    --slide-level=2 \

Change the theme with `-V theme = themeOfYourChoice`  
A list of themes can be found [here][themes]

Modify transition animation with `-V transition=[none/fade/slide/convex/concave/zoom]`  

Slide-level set to 2 allows for child slides to be spawned, Slide-level set to 1 only allows for parent slides. 

For an expansive list of customization options, refer to the revealjs [Configuration Options][config]


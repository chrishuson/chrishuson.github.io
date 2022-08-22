# Markdown notes

## Formatting

### markdown checkboxes

[x] this is a complete item

[ ] this is an incomplete item

*italics*
**bold**

(parentheses)

1. Numbered
1. lists

- Bullet
- lists

> Block quote
> text

    Code section:
    if return_code == TRUE
        then fail = 1


Table | Column 1 | Column 2
---|:---:|---:
Algebra | Symbols | 8, 9, 11
Geometry | Shapes | 7, 10

-------
(horizontal rule)

## Mathematics formulas (basic LaTeX)
LaTeX markdown is not being rendered by GitHub Pages' automatic process. A version converted to html by Markdown Preview Enhanced is [here](sandbox-rendered).

The Pythagorean formula and distance formula

$$a^2+b^2=c^2 \\[0.5cm]
d=\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}$$

## Geometry notation

$\triangle ABC$

$\overline{RS} \cong \overline{ST}$

## Rendering LaTeX code

[LaTeX package execution in markdown notes](latex-md-sandbox) (not working)
\tikz{\draw (0,0)--(2,1);}

## Graphics and images

![Geogebra triangle graph](https://raw.githubusercontent.com/chrishuson/course-files/master/Geom2023/graphics/06triangle.png)

![Rainfall plot](https://raw.githubusercontent.com/chrishuson/course-files/master/Geom2023/graphics/rainfall.png)

![Alt Dr. Huson](Chris_Huson.jpg)

html tags for image size

    <img src="image.png" width="200" height="100">

## Jupyter Notebooks

[link to Pandas Notes notebook](Pandas_Notes_Oct18)

[link to manual html export of Pandas Notes notebook](Pandas_Notes_manual_export)
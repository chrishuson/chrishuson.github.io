# Markdown notes

## Formatting

*italics*
**bold**

<p style="text-align:right; color:red"> 
    Your Right Aligned Text
</p>

<div class ="row">
    <button type="button" style= "margin-top : 20px; border-radius: 15px"
    class="btn btn-primary">View Profile</button>
</div>

1. Numbered
1. lists

- Bullet
- lists

[x] checklist completed item
[ ] this is an incomplete item

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

![Alt Dr. Huson](./images/Chris_Huson.jpg)

html tags for image size

<center>
<img src="./images/Chris_Huson.jpg" width="100" height="120">
</center>

## Slides

- "Fragments" <!-- .element: class="fragment" data-fragment-index="1" -->

## Jupyter Notebooks

[link to Pandas Notes notebook](Pandas_Notes_Oct18)

[link to manual html export of Pandas Notes notebook](Pandas_Notes_manual_export)
# Template for ASG white papers

[![Available on Overleaf](https://img.shields.io/badge/Available%20on-Overleaf-brightgreen.svg)](https://www.overleaf.com/read/qkcnfvhwhygv)

This is the content-only template used for authoring the ASG white papers, also [available on Overleaf](https://www.overleaf.com/read/qkcnfvhwhygv).
Although compiled into a PDF via `LaTeX`, the individual chapters are themselves plain-text Markdown files.

![A screenshot of the template in use on Overleaf](../../../images/ASG-White-Paper_template.png)

Note that Overleaf is used only to author the content, not to produce the final outputs (which will be PDF/print and HTML).
Once the content is frozen, following writing and reviewing, it will be used to generate the desired outputs.

## Files and content

The only `.tex` file in the template is `main.tex`, which includes all of the `LaTeX` packages needed to generate the PDF for (p)review.
It also defines the order of the chapters, as follows:

```latex
\markdownInput{summary.md}
\markdownInput{introduction.md}
\markdownInput{challenges.md}
\markdownInput{asg-contributions.md}
\markdownInput{recommendations.md}
\markdownInput{conclusions.md}
\markdownInput{acknowledgements.md}
```
 


## Use

To use this template on Overleaf, please copy all the files contained in this directory to your Overleaf project, replacing the default `main.tex` file with the one provided inn this directory.

Each chapter has its own file.
You may add new chapters as desired, but make sure to list them in the `main.tex` file for compilation.

You will need to use `LaTeX` comments instead of Markdown ones:

```latex
% A comment in $LaTeX$ to use with the “hybrid” Markdown files in Overleaf
```

It is also recommended to use [`Semantic Line Breaks`](https://sembr.org/), with new sentences beginning on new lines.
This makes for cleaner `diff`s of your source files:

```diff
- A new sentence is on a new line.
+ New sentences are on new lines.
```

### Adding images

…

### Adding references

…

[Zotero]

## Contribution

If you wish to suggest changes to this template, please submit a pull request to this repository with details about the proposed changes.
Please note that contribution requires that you adhere to the repository’s Code of Conduct.

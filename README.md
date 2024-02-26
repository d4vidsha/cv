# Resume

This is my personal resume written in LaTeX. It has been adapted from [Jake's Resume Template](https://www.overleaf.com/latex/templates/jakes-resume/syzfjbzwjncs).

```bash
latexmk --shell-escape -synctex=1 -interaction=nonstopmode -file-line-error -pdf -outdir=. -jobname=resume resume/main.tex
```

To install a package (such as `hyperref`), use the following command:

```bash
sudo tlmgr install hyperref
```

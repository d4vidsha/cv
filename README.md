# Resume

This is my personal resume written in LaTeX. It has been adapted from [Jake's Resume Template](https://www.overleaf.com/latex/templates/jakes-resume/syzfjbzwjncs).

```bash
latexmk --shell-escape -synctex=1 -interaction=nonstopmode -file-line-error -pdf -outdir=. -jobname=resume resume/main.tex
```

To install a package (such as `hyperref`), use the following command:

```bash
sudo tlmgr install hyperref
```

## How to rebase another branch

These instructions is specific to keeping the `intern-version` branch up-to-date with the `origin/HEAD` branch.

Replace `intern-version` with the branch you want to rebase.

```bash
git rebase --onto origin/HEAD $(git merge-base origin/HEAD intern-version) intern-version
git add resume.pdf
git rebase --continue
git push --force
```

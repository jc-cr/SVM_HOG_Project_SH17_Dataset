# SVM + HOG Project Report and Code

This is a SVM + HOG project I completed for class. 
It performed really bad on the COCO metrics, but had potential to be improved as IoUs after post-proccessing seem
to fall within the 0.4 range.

This repository contains the LaTeX build environment for my report and the source code for the project in the
[eval_code](/eval_code) dir.



## Build Req

- VS Code
- LaTeX Workshop extension

## LaTeX Build Env Setup

- Build the docker container: `cd .docker && docker compose build`
- Run the container: `docker compose up`

Now you can compile from the LaTeX workshop environment. 

If you need manual compilation for any reason you can do the following:
```
docker compose exec latex latexmk -pdf -outdir=/project/output /project/src/main.tex
```

# Compile with XeLaTeX
$pdf_mode = 5;
$xelatex = 'xelatex -synctex=1 -interaction=nonstopmode -file-line-error %O %S';
# The free Overleaf plan has a 10-second time limit. On every "Recompile"
# the book does not use an .aux file (\\nofiles), so xelatex runs only once.
$clean_ext = 'synctex.gz run.xml bbl';

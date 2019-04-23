# fANI2Tree
A R script to create an ANI-based UPGMA tree from fastANI output

## Prerequisites:

R

R-packages:
- tidyr
- ape
- phangorn

## Usage:

Create a all vs all comparison of your taxa of interest with fastANI (see https://github.com/ParBLiSS/FastANI for more information): 

```fastANI --q taxon_list.txt  --rl taxon_list.txt -o fastANI.output.txt```

Use fANI2Tree to convert the output to a UPGMA tree:

```Rscript fANI2Tree.R fastANI.output.txt your_treename.nwk```

And visualize your tree in FigTree (http://tree.bio.ed.ac.uk/software/figtree/) or your favorite treeviewer.

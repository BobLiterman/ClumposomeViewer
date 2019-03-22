# ClumposomeViewer

This is a Shiny app that takes as input:  
1) BED file with chromsomsome lengths  
2) BED file(s) with features of interest  
3) BED file with reference genomic regions of interest (optional)  

The basic pipeline is this:  

1) Use karyotypeR to generate a karyotype from the chrom BED  
2) Read in feature data and convert to sliding windows (user-settable values with slider)  
3) Import feature BED and calculate high density clusters ('high' defined by user)  
4) Extract cooridinates of high denisty regions, report back and cross reference with reference annotations if any exit  

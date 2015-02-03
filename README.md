# 4host


Microarray experiment, comparing P. capsici gene expression on four different host species. 
Infected leaf material was sampled at 16 hours post inoculation and analised using an agilent array

#####Create probeset
Probeset was generated by using all known P. capsici genes (Phyca11) and additionally, all in house predicted RxLR and CRN effectors.
Overlaps (e.g. a gene annotated in Phyca11 and our predictions) were removed and replaced by our effectors using `a script`

As input we used: `CRN.txt` (as published by Stam et al 2013), `Phyca11.fasta` (as published by Lamour et al 2013) and  `RxLR.txt` (wherefrom again?)

The resulting fasta file `something.fasta` was used in Agilent's earray software https://earray.chem.agilent.com/earray/ to generate the probeset. All earray files can be found in `Something`


#####Microarray analysis
The microarray data was analysed using `limma` from the `bioconductor` package. [here](http://www.bioconductor.org/packages/release/bioc/html/limma.html)




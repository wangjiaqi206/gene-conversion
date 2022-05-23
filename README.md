# gene-conversion
## Citations

- If you use the these methods to identify gene conversion, please cite:

  **Illegitimate recombination between** **duplicated** **genes contributes to the divergence of** **poplar and willow**.


## Contents

WCV：the Ks values between paralogous and orthologous gene pairs were 
used to infer possible whole gene conversion.

PCV: A combination of dynamic planning and phylogenetic analysis was used
to document the differences between two aligned bases from paralogous and 
orthologous genes for each genome. In averaged distance arrays, the paralogs 
in each species should be more distant if no PCV was involved.


## Installation

+ **Install ClustalW**

```console
wget http://www.clustal.org/download/current/clustalw-2.1.tar.gz
tar -zxvf clustalw-2.1.tar.gz
cd clustalw-2.1
./configure
make
```
+ **Install Perl**

https://www.perl.org/get.html

## Dependencies

Run the Perl package that gene-conversion depend on：

- [BioPerl ](https://metacpan.org/pod/BioPerl)

## command

+ The CV.paps, dna.paps, and out.cv folders are required to run gene-conversion
+ After running WCV, the files in dna.paps are used to run PCV
~~~bash
## Run WCV
perl WCV.Ptr.and.Sbr.pl Ptr_Sbr.quartet.txt Ptr Sbr

## Run PCV
perl PCV.Sbr.and.Ptr.pl Sbr_Ptr.quartet
~~~


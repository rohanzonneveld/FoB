data/vep/HGVS_2014_VEP_baseline.tsv data/BLOSUM62.txt -o data/vep/HGVS_2014_baseline_scores.tsv 

-ipred data/vep/HGVS_2014_baseline_scores.tsv -ibench data/HGVS_2014_benchmark.tsv -color -o output/ROC_plot_baseline_test.png

-ipred data/vep/HGVS_2014_baseline_scores.tsv -ipred data/vep/HGVS_2014_polyphen_scores.tsv -ipred data/vep/HGVS_2014_sift_scores.tsv -ibench data/HGVS_2014_benchmark.tsv -o output/ROC_plot_all_test.png

-itsv output/xy/polyphen_2014.tsv -itsv output/xy/polyphen_2020\ small.tsv -itsv output/xy/polyphen_2020\ big.tsv -o output/ROC_plot_comparison_polyphen.png
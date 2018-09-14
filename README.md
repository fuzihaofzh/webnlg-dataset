# WebNLG Dataset Summary

This repository presents the evolution of the WebNLG corpus.

Each folder contains *the same data* in two formats: `xml` and `json`.

1. `release_v2`
	
	It is the latest release.

	It includes release_v1 and test data (seen categories) from the WebNLG challenge.

	We split it into train/dev/test, ensuring equal representation of DBpedia categories and tripleset sizes.

	Tree shapes and types (_sibling, chain, mixed_) were added for each input RDF tree.

2. `release_v2_constrained`

	It has the same data as release_v2.

	The split into train/dev/test is more challenging. That split ensures that a triple occurring in train/dev is not present in test (more info in the INLG 2018 paper below).

3. `release_v1`

	It matches Final Release (Larger Dataset) on the [challenge website](http://webnlg.loria.fr/pages/results.html).

	It doesn't include test data (seen categories) from the challenge.

	No split into train/dev/test was provided.
	
	Covers 15 DBpedia categories.

4. `webnlg_challenge_2017`

	Contains the data used in the [WebNLG Challenge 2017](http://webnlg.loria.fr/pages/results.html).
	
	Covers 10 DBpedia categories (the _City_ category only partially). 

## Documentation

[http://webnlg.loria.fr/pages/docs.html](http://webnlg.loria.fr/pages/docs.html)

## Publications
* [Creating Training Corpora for NLG Micro-Planners](http://www.aclweb.org/anthology/P17-1017). C. Gardent, A. Shimorina, S. Narayan, L. Perez-Beltrachini. ACL 2017.

* [The WebNLG Challenge: Generating Text from RDF Data](http://aclweb.org/anthology/W17-3518). C. Gardent, A. Shimorina, S. Narayan, L. Perez-Beltrachini. INLG 2017.

* Handling Rare Items in Data-to-Text Generation. A. Shimorina, C. Gardent. INLG 2018 (to appear).

## Citing

* If you use the WebNLG corpus, cite

```
@InProceedings{gardent2017creating,
  author = 	"Gardent, Claire
		and Shimorina, Anastasia
		and Narayan, Shashi
		and Perez-Beltrachini, Laura",
  title = 	"Creating Training Corpora for NLG Micro-Planners",
  booktitle = 	"Proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)    ",
  year = 	"2017",
  publisher = 	"Association for Computational Linguistics",
  pages = 	"179--188",
  location = 	"Vancouver, Canada",
  doi = 	"10.18653/v1/P17-1017",
  url = 	"http://www.aclweb.org/anthology/P17-1017"
}
```

* If you use _release_v2_constrained_ in particular, cite

```
@InProceedings{shimorina2018handling,
  author = 	"Shimorina, Anastasia
		and Gardent, Claire",
  title = 	"Handling Rare Items in Data-to-Text Generation",
  booktitle = 	"Proceedings of the 11th International Conference on Natural Language Generation",
  year = 	"2018",
  publisher = 	"Association for Computational Linguistics",
  location = 	"Tilburg, The Netherlands"
}
```

## License
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

## Contact
* webnlg2017@inria.fr
* or create an issue in this repository
 

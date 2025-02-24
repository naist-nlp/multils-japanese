# MultiLS-Japanese
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

MultiLS-Japanese is a lexical complexity prediction (LCP) and lexical simplification (LS) dataset for Japanese.

This repository provides:

1. Additional data for the **original annotation**, which was used to evaluate the MLSP 2024 shared task:
    - [LCP](annotator_profiles/lcp_profiles.tsv) and [LS](annotator_profiles/ls_profiles.tsv) annotator profiles. Note that each instance in both trial and test data was annotated by the the same annotators.
    - [Unaggregated trial](data/lcp_unaggregated_trial.tsv) and [test]((data/lcp_unaggregated_test.tsv)) ratings for LCP that can be merged with the Japanese dataset using the `id` column.
    - [Empty Excel templates](annotation_templates) used for annotation including our annotation guidelines and the exact questions we asked in the annotator profiles.

2. **Non-Chinese/Korean L1 replication** of the LCP trial set:
    - [Annotator profiles](annotator_profiles/replication_lcp_profiles.tsv).
    - [Ratings](data/replication_lcp_trial.tsv) (both unaggregated and aggregated values).

3. **Chinese L1 reannotation** of the LCP trial set:
    - [Annotator profiles](annotator_profiles/chinese_l1_lcp_profiles.tsv).
    - [Ratings](data/chinese_l1_lcp_trial.tsv) (both unaggregated and aggregated values).

The last two trial set annotations were used for analysis in “Difficult for Whom? A Study of Japanese Lexical Complexity” ([Nohejl et al., 2024](https://aclanthology.org/2024.tsar-1.8)). Only the original data was used for the MLSP shared task ([Shardlow et al., 2024](https://aclanthology.org/2024.bea-1.51)).

## The LS and LCP Data

Please get the data for all languages, including Japanese (original annotation), from the [MLSP2024](https://huggingface.co/datasets/MLSP2024/MLSP2024) dataset on Hugging Face Hub. This `multils-japanese` repository only provides additional data specific for the Japanese subset of MultiLS (MLSP2024) dataset.

## Papers

The MultiLS-Japanese dataset was created by Adam Nohejl, Akio Haykawa, and Yusuke Ide. We are working on a paper dedicated to the dataset. In the mean time, please refer to the following papers and cite them when using the dataset.

### MultiLS-Japanese: Analysis and Additional Annotation 

[Paper](https://aclanthology.org/2024.tsar-1.8)
```
@inproceedings{nohejl-etal-2024-difficult,
  title = {Difficult for {{Whom}}? {{A Study}} of {{Japanese Lexical Complexity}}},
  author = {Nohejl, Adam and Hayakawa, Akio and Ide, Yusuke and Watanabe, Taro},
  booktitle = "Proceedings of the Third Workshop on Text Simplification, Accessibility and Readability (TSAR 2024)",
  year = {2024}, url = "https://aclanthology.org/2024.tsar-1.8",
}
```

### MultiLS (all MLSP2024 data): Shared Task Report and Dataset
[Paper](https://aclanthology.org/2024.bea-1.51)
```
@inproceedings{shardlow2024bea,
  title={{The BEA 2024 Shared Task on the Multilingual Lexical Simplification Pipeline}},
  author={Shardlow, Matthew and Alva-Manchego, Fernando and Batista-Navarro, Riza and Bott, Stefan and Calderon Ramirez, Saul and Cardon, Rémi and François, Thomas and Hayakawa, Akio and Horbach, Andrea and Huelsing, Anna and Ide, Yusuke and Imperial, Joseph Marvin and Nohejl, Adam and North, Kai and Occhipinti, Laura and Peréz Rojas, Nelson and Raihan, Nishat and Ranasinghe, Tharindu and Solis Salazar, Martin and \v{S}tajner, Sanja and Zampieri, Marcos and Saggion, Horacio},
  booktitle={Proceedings of the 19th Workshop on Innovative Use of NLP for Building Educational Applications (BEA)},
year={2024}
}
```

### MultiLS (all MLSP2024 data): Dataset Creation
[Paper](https://aclanthology.org/2024.readi-1.4)
```
@inproceedings{shardlow2024readi,
  title={{An Extensible Massively Multilingual Lexical Simplification Pipeline Dataset using the MultiLS Framework}},
  author={Shardlow, Matthew and Alva-Manchego, Fernando and Batista-Navarro, Riza and Bott, Stefan and Calderon Ramirez, Saul and Cardon, Rémi and François, Thomas and Hayakawa, Akio and Horbach, Andrea and Huelsing, Anna and Ide, Yusuke and Imperial, Joseph Marvin and Nohejl, Adam and North, Kai and Occhipinti, Laura and Peréz Rojas, Nelson and Raihan, Nishat and Ranasinghe, Tharindu and Solis Salazar, Martin and Zampieri, Marcos and Saggion, Horacio},
  booktitle={Proceedings of the 3rd Workshop on Tools and Resources for People with REAding DIfficulties (READI)},
year={2024}
}
```

## Related Work

### [JaLeCoN](https://github.com/naist-nlp/jalecon), a Dataset of Japanese Lexical Complexity for Non-Native Readers

[Paper](https://aclanthology.org/2023.bea-1.40). The annotation was done with a slightly different scale and in a dense setting.

```
@inproceedings{ide2023,
  title     = "Japanese Lexical Complexity for Non-Native Readers: A New Dataset",
  author    = "Ide, Yusuke and Mita, Masato and Nohejl, Adam and Ouchi, Hiroki and Watanabe, Taro",
  booktitle = "Proceedings of the Eighteenth Workshop on Innovative Use of {NLP} for Building Educational Applications",
  month     = July,
  year      = 2023,
  publisher = "Association for Computational Linguistics",
}
```

### MultiLS Framework

[Paper](https://arxiv.org/abs/2402.14972)

```
@article{north2024multils,
  title={MultiLS: A Multi-task Lexical Simplification Framework},
  author={North, Kai and Ranasinghe, Tharindu and Shardlow, Matthew and Zampieri, Marcos},
  journal={arXiv preprint arXiv:2402.14972}, year={2024}
}
```

### MultiLS-SP/CA: Spanish and Catalan Datasets

[Paper](https://arxiv.org/abs/2404.07814)

```
@misc{bott2024multilsspca,
      title={MultiLS-SP/CA: Lexical Complexity Prediction and Lexical Simplification Resources for Catalan and Spanish},
      author={Stefan Bott and Horacio Saggion and Nelson Peréz Rojas and Martin Solis Salazar and Saul Calderon Ramirez},
      year={2024},
      eprint={2404.07814},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

You may also be interested in Japanese lexical simplification datasets targeting native speakers (by different authors):

- Controlled and Balanced Dataset for Japanese Lexical Simplification ([Kodaira et al., 2016](https://aclanthology.org/P16-3001)): [dataset](https://github.com/KodairaTomonori/EvaluationDataset)
- Evaluation Dataset and System for Japanese Lexical Simplification ([Kajiwara and Yamamoto, 2015](http://www.aclweb.org/anthology/P15-3006): [dataset](https://www.jnlp.org/GengoHouse/snow/e4)



## License

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa]. Please, cite [our](https://aclanthology.org/2024.tsar-1.8) [papers](https://aclanthology.org/2024.bea-1.51) if you use the data.

See the sources and license information for [trial set](LICENSE_trial.md) and [test set](LICENSE_test.md) for details.

[cc-by-sa]: https://creativecommons.org/licenses/by-sa/4.0/


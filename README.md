# MultiLS-Japanese
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

MultiLS-Japanese is a lexical complexity prediction (LCP) and lexical simplification (LS) dataset for Japanese. This repository provides:

- LCP and LS [annotator profiles](annotator_profiles). Note that each instance in both trial and test data was annotated by the the same annotators.
- [Unaggregated ratings](unaggregated_data) for LCP that can be merged with the Japanese dataset using the `id` column.
- [Empty Excel templates](annotation_templates) used for annotation including our annotation guidelines and the exact questions we asked in the annotator profiles.


## The LS and LCP data

Please use the Japanese data in [MLSP2024](https://huggingface.co/datasets/MLSP2024/MLSP2024) dataset on Hugging Face Hub. This repository only provides additional information specific for the Japanese subset of MultiLS (MLSP2024) dataset.

If you use the LS and LCP data or the data and information provided by this repository, please cite our papers:

### Shared Task Report and Dataset
[Paper](https://aclanthology.org/2024.bea-1.51)
```
@inproceedings{shardlow2024bea,
title={{The BEA 2024 Shared Task on the Multilingual Lexical Simplification Pipeline}},
author={Shardlow, Matthew and Alva-Manchego, Fernando and Batista-Navarro, Riza and Bott, Stefan and Calderon Ramirez, Saul and Cardon, Rémi and François, Thomas and Hayakawa, Akio and Horbach, Andrea and Huelsing, Anna and Ide, Yusuke and Imperial, Joseph Marvin and Nohejl, Adam and North, Kai and Occhipinti, Laura and Peréz Rojas, Nelson and Raihan, Nishat and Ranasinghe, Tharindu and Solis Salazar, Martin and \v{S}tajner, Sanja and Zampieri, Marcos and Saggion, Horacio},
booktitle={Proceedings of the 19th Workshop on Innovative Use of NLP for Building Educational Applications (BEA)},
year={2024}
}
```

### Dataset Creation
[Paper](https://aclanthology.org/2024.readi-1.4)
```
@inproceedings{shardlow2024readi,
title={{An Extensible Massively Multilingual Lexical Simplification Pipeline Dataset using the MultiLS Framework}},
author={Shardlow, Matthew and Alva-Manchego, Fernando and Batista-Navarro, Riza and Bott, Stefan and Calderon Ramirez, Saul and Cardon, Rémi and François, Thomas and Hayakawa, Akio and Horbach, Andrea and Huelsing, Anna and Ide, Yusuke and Imperial, Joseph Marvin and Nohejl, Adam and North, Kai and Occhipinti, Laura and Peréz Rojas, Nelson and Raihan, Nishat and Ranasinghe, Tharindu and Solis Salazar, Martin and Zampieri, Marcos and Saggion, Horacio},
booktitle={Proceedings of the 3rd Workshop on Tools and Resources for People with REAding DIfficulties (READI)},
year={2024}
}
```

## Related Papers

### [JaLeCoN](https://github.com/naist-nlp/jalecon), a Dataset of Japanese Lexical Complexity for Non-Native Readers

[Paper](https://aclanthology.org/2023.bea-1.40). The annotation was done with a slightly different scale and in a dense setting.

```
@inproceedings{ide2023,
  title     = "Japanese Lexical Complexity for Non-Native Readers: A New Dataset",
  booktitle = "Proceedings of the Eighteenth Workshop on Innovative Use of {NLP} for Building Educational Applications",
  author    = "Ide, Yusuke and Mita, Masato and Nohejl, Adam and Ouchi, Hiroki and Watanabe, Taro",
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
  journal={arXiv preprint arXiv:2402.14972},
  year={2024}
}
```

### Spanish and Catalan Datasets

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

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa]. Please see the sources and license information for [trial set](LICENSE_trial.md) and [test set](LICENSE_test.md) for details.

[cc-by-nc-sa]: https://creativecommons.org/licenses/by-nc-sa/4.0/


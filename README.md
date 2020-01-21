# BioBERT Pre-trained Weights

This repository provides pre-trained weights of BioBERT, a language representation model for biomedical domain, especially designed for biomedical text mining tasks such as biomedical named entity recognition, relation extraction, question answering, etc.
Please refer to our paper [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://arxiv.org/abs/1901.08746) for more details.

## Downloading pre-trained weights
Go to [releases](https://github.com/naver/biobert-pretrained/releases) section of this repository or click links below to download pre-trained weights of BioBERT.
We provide three combinations of pre-trained weights: BioBERT (+ PubMed), BioBERT (+ PMC), and BioBERT (+ PubMed + PMC).
Pre-training was based on the [original BERT code](https://github.com/google-research/bert) provided by Google, and training details are described in our paper. Currently available versions of pre-trained weights are as follows:

* **[BioBERT-Base v1.1 (+ PubMed 1M)](https://drive.google.com/file/d/1R84voFKHfWV9xjzeLzWBbmY1uOMYpnyD/view?usp=sharing)** - based on BERT-base-Cased (same vocabulary)
* **[BioBERT-Large v1.1 (+ PubMed 1M)](https://drive.google.com/file/d/1GJpGjQj6aZPV-EfbiQELpBkvlGtoKiyA/view?usp=sharing)** - based on BERT-large-Cased (custom 30k vocabulary), [NER/QA Results](https://github.com/dmis-lab/biobert/wiki/BioBERT-Large-Results)
* **[BioBERT-Base v1.0 (+ PubMed 200K)](https://drive.google.com/file/d/17j6pSKZt5TtJ8oQCDNIwlSZ0q5w7NNBg/view?usp=sharing)** - based on BERT-base-Cased (same vocabulary)
* **[BioBERT-Base v1.0 (+ PMC 270K)](https://drive.google.com/file/d/1LiAJklso-DCAJmBekRTVEvqUOfm0a9fX/view?usp=sharing)** - based on BERT-base-Cased (same vocabulary)
* **[BioBERT-Base v1.0 (+ PubMed 200K + PMC 270K)](https://drive.google.com/file/d/1jGUu2dWB1RaeXmezeJmdiPKQp3ZCmNb7/view?usp=sharing)** - based on BERT-base-Cased (same vocabulary)

Make sure to specify the versions of pre-trained weights used in your works.
If you have difficulty choosing which one to use, we recommend using **BioBERT-Base v1.1 (+ PubMed 1M)** or **BioBERT-Large v1.1 (+ PubMed 1M)** depending on your GPU resources.
Note that for BioBERT-Base, we are using WordPiece vocabulary (`vocab.txt`) provided by Google as any new words in biomedical corpus can be represented with subwords (for instance, Leukemia => Leu + ##ke + ##mia).
More details are in the closed [issue #1](https://github.com/naver/biobert-pretrained/issues/1).

## Pre-training corpus
We do not provide pre-processed version of each corpus. However, each pre-training corpus could be found in the following links:
*   **`PubMed Abstracts1`**: ftp://ftp.ncbi.nlm.nih.gov/pubmed/baseline/
*   **`PubMed Abstracts2`**: ftp://ftp.ncbi.nlm.nih.gov/pubmed/updatefiles/
*   **`PubMed Central Full Texts`**: ftp://ftp.ncbi.nlm.nih.gov/pub/pmc/oa_bulk/

Estimated size of each corpus is 4.5 billion words for **`PubMed Abstracts1`** + **`PubMed Abstracts2`**, and 13.5 billion words for **`PubMed Central Full Texts`**.

## Fine-tuning BioBERT
To fine-tunine BioBERT on biomedical text mining tasks using provided pre-trained weights, refer to the [DMIS GitHub repository for BioBERT](https://github.com/dmis-lab/biobert).

## Citation
```
@article{10.1093/bioinformatics/btz682,
    author = {Lee, Jinhyuk and Yoon, Wonjin and Kim, Sungdong and Kim, Donghyeon and Kim, Sunkyu and So, Chan Ho and Kang, Jaewoo},
    title = "{BioBERT: a pre-trained biomedical language representation model for biomedical text mining}",
    journal = {Bioinformatics},
    year = {2019},
    month = {09},
    issn = {1367-4803},
    doi = {10.1093/bioinformatics/btz682},
    url = {https://doi.org/10.1093/bioinformatics/btz682},
}
```

## Contact information
For help or issues using pre-trained weights of BioBERT, please submit a GitHub issue. Please contact Jinhyuk Lee
(`lee.jnhk@gmail.com`), or Sungdong Kim (`sungdong.kim@navercorp.com`) for communication related to pre-trained weights of BioBERT.

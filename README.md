# BioBERT Pre-trained Weights

This repository provides pre-trained weights of BioBERT, a language representation model for biomedical domain, especially designed for biomedical text mining tasks such as biomedical named entity recognition, relation extraction, question answering, etc. Please refer to our paper [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://arxiv.org/abs/1901.08746) for more details.

## Downloading pre-trained weights
Go to [releases](https://github.com/naver/biobert-pretrained/releases) section of this repository, and download pre-trained weights of BioBERT. We provide three combinations of pre-trained BioBERT: Wiki + Books + PubMed, Wiki + Books + PMC, and Wiki + Books + PubMed + PMC. Pre-training was based on the [original BERT code](https://github.com/google-research/bert) provided by Google, and details are described in our paper.

## Pre-training corpus
We do not provide pre-processed version of each corpus. However, each pre-training corpus could be found in the following links:
*   **`PubMed Abstracts1`**: ftp://ftp.ncbi.nlm.nih.gov/pubmed/baseline/
*   **`PubMed Abstracts2`**: ftp://ftp.ncbi.nlm.nih.gov/pubmed/updatefiles/
*   **`PubMed Central Full Texts`**: ftp://ftp.ncbi.nlm.nih.gov/pub/pmc/oa_bulk/

Estimated size of each corpus is 4.5 billion words for **`PubMed Abstracts1`** + **`PubMed Abstracts2`**, and 13.5 billion words for **`PubMed Central Full Texts`**.

## Fine-tuning BioBERT
To fine-tunine BioBERT on biomedical text mining tasks using provided pre-trained weights, refer to the [DMIS GitHub repository for BioBERT](https://github.com/dmis-lab/biobert).

## Citation
For now, cite [the Arxiv paper](https://arxiv.org/abs/1901.08746):
```
@article{lee2019biobert,
  title={BioBERT: a pre-trained biomedical language representation model for biomedical text mining},
  author={Lee, Jinhyuk and Yoon, Wonjin and Kim, Sungdong and Kim, Donghyeon and Kim, Sunkyu and So, Chan Ho and Kang, Jaewoo},
  journal={arXiv preprint arXiv:1901.08746},
  year={2019}
}
```

## Contact information
For help or issues using pre-trained weights of BioBERT, please submit a GitHub issue. Please contact Jinhyuk Lee
(`lee.jnhk@gmail.com`), or Sungdong Kim (`sungdong.kim@navercorp.com`) for communication related to pre-trained weights of BioBERT.

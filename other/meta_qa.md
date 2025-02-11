# MetaQA 

**MoviE Text Audio QA (MetaQA)**<sup>[[1]](#myfootnote1)</sup> contains more than 400K questions for both single and multi-hop reasoning, and provides more realistic text and audio versions. MetaQA serves as a comprehensive extension of WikiMovies., in English language. Containing 400,000+ in Text, MP3 file format.

According to the original paper, there are three versions of this dataset: Vanilla, NTM and Audio. Vanilla is a composed of original WikiMovies as 1-hop dataset, 21 types of 2-hop questions and 15 types of 3-hop questions. NTM is generated by translating the Vanilla set using machine translation models. Audio subset is generated by  audio datasets with the help of text-to-speech (TTS) system.

If not specified, dataset below refers to Vanilla set of MetaQA.

This dataset can be downloaded via the [link](https://github.com/yuyuz/MetaQA).
Note that this dataset is divided into 1-hop, 2-hop and 3-hop in the original paper: [Variational reasoning for question answering with knowledge graph](https://arxiv.org/pdf/1709.04071.pdf).

## 1-hop

### Leaderboard

|       Model / System        | Year | Hits@1 |  F1 | Exact Match |                               Language                             |                                       Reported by                                       |
|:---------------------------:|:----:|:------:|:------:|:-----------:|:------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|
|           SSKGQA            | 2022 |  99.1  |  - |  -  |   EN    |   [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|           NRQA              | 2022 |  98.1  | - |  -  |   EN  | [Guo et al.](https://link.springer.com/content/pdf/10.1007/s10489-022-03927-0.pdf)  |
|            DCRN             | 2022 |  97.5  | - |   -      |     EN  |   [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|             VRN             | 2017 |  97.5  |   - |    -   |     EN      |     [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)  |
|          EmbedKGQA          | 2020 |  97.5  |   - |    -      |     EN      |   [Saxena et al.](https://aclanthology.org/2020.acl-main.412.pdf) |
|            QAGCN            | 2022 |  97.3  |  - |     -      |     EN      |    [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)  |
|            NSM+p            | 2021 |  97.3  |   - |    -      |     EN      |    [He et al.](https://arxiv.org/pdf/2101.03737.pdf)   |
|           QNRKGQA           | 2022 |  97.3  |   - |    -    |     EN   |    [Ma et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_11)     |
|            NSM+h            | 2021 |  97.2  |  - |     -      |     EN      |                [He et al.](https://arxiv.org/pdf/2101.03737.pdf)   |
|   Edge-aware GNN            | 2022 |  97.2  | 98.5 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   GlobalGraph               | 2022 |  99.0  | 97.6 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   2HR-DR                    | 2022 |  98.8  | 97.3 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   SGReader                  | 2022 |  96.7  | 96.0 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   GRAFT-Net                 | 2022 |  97.4  | 91.0 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|             NSM             | 2021 |  97.1  |  - |     -      |     EN      |                [He et al.](https://arxiv.org/pdf/2101.03737.pdf)   |
|             SRN             | 2020 |  97.0  |   - |    -      |     EN      |          [Qiu et al.](https://dl.acm.org/doi/10.1145/3336191.3371812) |
|          GraftNet           | 2018 |  97.0  |  - |   -      |     EN      |               [Sun et al.](https://aclanthology.org/D18-1455.pdf)  |
|           PullNet           | 2019 |  97.0  |   - |    -      |     EN      |               [Sun et al.](https://arxiv.org/pdf/1904.09537.pdf)   |
|           MINERVA           | 2022 |  96.3  |   - |    -      |     EN      |               [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)  |
|           ReifKB            | 2020 |  96.2  |   - |    -      |     EN      |              [Cohen et al.](https://arxiv.org/pdf/2002.06115.pdf)  |
|          KV-MemNN           | 2022 |  96.2  |   - |    -      |     EN      |   [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|         TransferNet         | 2022 |  96.0  |   - |    -      |     EN      |   [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
| Borders et al. 's QA system | 2017 |  95.7  |   - |    -      |     EN      |              [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)  |
|          KV-MemNN           | 2017 |  95.8  |   - |    -      |     EN      |              [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)  |
|          AlAgha, 2022       | 2022 |  95.4  |   - |    -      |     EN      |    [AlAgha, 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9834917)|
|   KGQA Based on Query Path Generation| 2022 |  93.9  |  - |    - |   EN  |  [Yang et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_12)|
|             IRN             | 2022 |  85.9  |   - |    -      |     EN      |      [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)  |
|    Supervised embedding     | 2017 |  54.4  |   - |    -      |     EN      |              [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)  |
|            T5+KG            | 2022 |   -    |   - |  71.47    |     EN      |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |
|             T5              | 2022 |   -    |   - |  24.5     |     EN      |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |
|            T5+C4            | 2022 |   -    |  - |   23.53    |     EN      |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |

## 2-hop

### Leaderboard

|       Model / System        | Year | Hits@1 |  F1 | Exact Match |                               Language                             |                                       Reported by                                       |
|:---------------------------:|:----:|:------:|:------:|:-----------:|:------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|
|   KGQA Based on Query Path Generation| 2022 |  99.9  | - |     -    |   EN   |   [Yang et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_12)|
|           PullNet           | 2019 |  99.9  |  - |     -      |     EN     |       [Sun et al.](https://arxiv.org/pdf/1904.09537.pdf)        |
|            DCRN             | 2022 |  99.9  |   - |    -      |   EN    |    [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf)        |
|             NSM             | 2021 |  99.9  |  - |     -      |  EN      |              [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|            NSM+p            | 2021 |  99.9  |  - |     -      |    EN      |              [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|            NSM+h            | 2021 |  99.9  | - |      -      |        EN       |              [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|            QAGCN            | 2022 |  99.9  | - |      -      |   EN        |            [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|           QNRKGQA           | 2022 |  99.9  |  - |     -      |     EN      |    [Ma et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_11)     |
|          QNRKGQA+h          | 2022 |  99.9  |  - |     -      |   EN   |    [Ma et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_11)     |
|           SSKGQA            | 2022 |  99.7  |  - |     -      |      EN      | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|          EmbedKGQA          | 2020 |  98.8  |  - |     -      |        EN    |      [Saxena et al.](https://aclanthology.org/2020.acl-main.412.pdf)       |
|         TransferNet         | 2022 |  98.5  |  - |     -      |     EN         | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|            NRQA             | 2022 |  97.5  |  - |     -      |    EN    | [Guo et al.](https://link.springer.com/content/pdf/10.1007/s10489-022-03927-0.pdf)  |
|   Edge-aware GNN            | 2022 |  96.8  | 93.7 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   GlobalGraph               | 2022 |   95.5  | 83.0 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   2HR-DR                    | 2022 |   93.7  | 81.4 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   SGReader                  | 2022 |   80.7  | 79.8 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|   GraftNet                  | 2022 |   94.8  | 72.7 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|         ReifKB+mask         | 2020 |  95.4  |   - |    -      |       EN        |              [Cohen et al.](https://arxiv.org/pdf/2002.06115.pdf)              |
|             SRN             | 2020 |  95.1  |  - |     -      |      EN     |        [Qiu et al.](https://dl.acm.org/doi/10.1145/3336191.3371812)        |
|          GraftNet           | 2018 |  94.8  |  - |     -      |       EN      |            [Sun et al.](https://aclanthology.org/D18-1455.pdf) |   
|          AlAgha, 2022        | 2022 |  94.1  | - |      -     |  EN    | [AlAgha, 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9834917)            |
|           MINERVA           | 2022 |  92.9  |  - |     -      |          EN       |            [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|             VRN             | 2017 |  89.9  |  - |     -      |          EN       |       [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)            |
|             VRN             | 2022 |  89.2  | - |      -      |            EN       | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|          KV-MemNN           | 2022 |  82.7  |  - |     -      |              EN    | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
| Borders et al. 's QA system | 2017 |  81.8  |  - |     -      |             EN      |            [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)          |
|           ReifKB            | 2020 |  81.1  |  - |     -      |       EN  |              [Cohen et al.](https://arxiv.org/pdf/2002.06115.pdf)              |
|   KV-MemNN                  | 2022 |  76.0  |  - |    -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|             IRN             | 2022 |  71.3  |  - |     -      |         EN     |            [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|    Supervised embedding     | 2017 |  29.1  | - |      -      |           EN    |             [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)           |
|          KV-MemNN           | 2017 |  25.1  |  - |     -      |         EN               |        [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)        |
|            T5+KG            | 2022 |   -    |  - |   33.57    |             EN            |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |
|            T5+C4            | 2022 |   -    |  - |   32.78    |          EN                |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       
|             T5              | 2022 |   -    |  - |   32.65    |            EN               |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |

## 3-hop

### Leaderboard

|       Model / System        | Year | Hits@1 |  F1 |  Exact Match |                                Language                                |                                       Reported by                                       |
|:---------------------------:|:----:|:------:|:------:|:-----------:|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|
|           SSKGQA            | 2022 |  99.6  |  -   |  -  |   EN    | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|            DCRN             | 202  |  99.3  |  -   | -   |    EN   | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|             NSM             | 2021 |  98.9  |  -   |  -  |    EN        |             [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|            NSM+p            | 2021 |  98.9  |  -   | -   |     EN      |        [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|            NSM+h            | 2021 |  98.9  |  -  |  -   |      EN      |             [He et al.](https://arxiv.org/pdf/2101.03737.pdf)              |
|           QNRKGQA           | 2022 |  98.9  |   -  |  -  |     EN       |    [Ma et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_11)     |
|          QNRKGQA+h          | 2022 |  98.9  |   -  |  -  |     EN     |    [Ma et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_11)     |
|   KGQA Based on Query Path Generation| 2022 |  98.5  |  -  |  -   |  EN   |    [Yang et al.](https://link.springer.com/chapter/10.1007/978-3-031-10983-6_12)|
|            QAGCN            | 2022 |  97.6  |   -  |  -   |    EN        |       [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|   Edge-aware GNN            | 2022 |  96.3  | 91.0 |       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|            NRQA             | 2022 |  96.1  |    -  |  -     |    EN    | [Guo et al.](https://link.springer.com/content/pdf/10.1007/s10489-022-03927-0.pdf)  |
|          EmbedKGQA          | 2020 |  94.8  |      -  |  -      |      EN       |      [Saxena et al.](https://aclanthology.org/2020.acl-main.412.pdf)       |
|         TransferNet         | 2022 |  94.7  |     -  |  -     |     EN      | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|          AlAgha, 2022       | 2022 |  93.4  |    -  |  -      |     EN      |        [AlAgha, 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9834917)|
|           PullNet           | 2022 |  91.4  |    -  |  -      |        EN    |             [Sun et al.](https://arxiv.org/pdf/1904.09537.pdf)             |
|   GlobalGraph               | 2022 |  81.4  | 62.4|       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|         ReifKB+mask         | 2020 |  79.7  |    -  |  -      |      EN       |            [Cohen et al.](https://arxiv.org/pdf/2002.06115.pdf)            |
|   GraftNet                   | 2022 |  77.8 | 56.1|       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|          GraftNet           | 2022 |  77.7  |    -  |  -      |       EN         | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|          GraftNet           | 2018 |  77.2  |     -  |  -      |       EN           |            [Sun et al.](https://aclanthology.org/D18-1455.pdf)             |
|             SRN             | 2020 |  75.2  |    -  |  -     |      EN         |        [Qiu et al.](https://dl.acm.org/doi/10.1145/3336191.3371812)        |
|           ReifKB            | 2020 |  72.3  |     -  |  -      |       EN          |            [Cohen et al.](https://arxiv.org/pdf/2002.06115.pdf)            |
|             VRN             | 2017 |  62.5  |     -  |  -      |       EN      |            [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)            |
|   SGReader                   | 2022 |  61.0 | 58.0|       -    |     EN      |   [Zhang et al.](https://downloads.hindawi.com/journals/cin/2022/4734179.pdf) |
|           MINERVA           | 2022 |  55.2  |    -  |  -      |     EN         |            [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|          KV-MemNN           | 2022 |  48.9  |    -  |  -     |      EN            | [Mingchen Li and Jonathan Shihao Ji](https://arxiv.org/pdf/2204.10194.pdf) |
|             IRN             | 2022 |  35.6  |    -  |  -     |       EN      |            [Wang et al.](https://arxiv.org/pdf/2206.01818.pdf)             |
|    Supervised embedding     | 2017 |  28.9  |    -  |  -     |      EN       |            [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)            |
| Borders et al. 's QA system | 2017 |  28.4  |   -  |  -   |        EN      |            [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)            |
|          KV-MemNN           | 2017 |  10.1  |    -  |  -     |         EN         |            [Zhang et al.](https://arxiv.org/pdf/1709.04071.pdf)            |
|            T5+KG            | 2022 |   -  |  -    |    43.41    |      EN        |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |
|             T5              | 2022 |   -  |  -    |    42.31    |       EN         |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |
|            T5+C4            | 2022 |   -  |  -     |    39.66    |        EN       |       [Moiseev et al.](https://arxiv.org/pdf/2205.08184.pdf)       |



## References 
<a name="myfootnote1">[1]</a> Zhang, Yuyu, Hanjun Dai, Zornitsa Kozareva, Alexander J. Smola, and Le Song. [Variational reasoning for question answering with knowledge graph.](https://arxiv.org/pdf/1709.04071.pdf) In Thirty-Second AAAI Conference on Artificial Intelligence. 2018.




[Go back to the README](../README.md)


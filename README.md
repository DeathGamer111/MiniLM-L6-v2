---
pipeline_tag: sentence-similarity
tags:
- sentence-transformers
- feature-extraction
- sentence-similarity
- mteb
language: en
license: apache-2.0
datasets:
- s2orc
- flax-sentence-embeddings/stackexchange_xml
- MS Marco
- gooaq
- yahoo_answers_topics
- code_search_net
- search_qa
- eli5
- snli
- multi_nli
- wikihow
- natural_questions
- trivia_qa
- embedding-data/sentence-compression
- embedding-data/flickr30k-captions
- embedding-data/altlex
- embedding-data/simple-wiki
- embedding-data/QQP
- embedding-data/SPECTER
- embedding-data/PAQ_pairs
- embedding-data/WikiAnswers
model-index:
- name: all-MiniLM-L6-v2
  results:
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (en)
      config: en
      split: test
      revision: 2d8a100785abf0ae21420d2a55b0c56e3e1ea996
    metrics:
    - type: accuracy
      value: 64.14925373134331
    - type: ap
      value: 27.237875815186907
    - type: f1
      value: 58.03105716318715
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_polarity
      name: MTEB AmazonPolarityClassification
      config: default
      split: test
      revision: 80714f8dcf8cefc218ef4f8c5a966dd83f75a0e1
    metrics:
    - type: accuracy
      value: 62.582975
    - type: ap
      value: 58.26562634146188
    - type: f1
      value: 62.304673961004156
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (en)
      config: en
      split: test
      revision: c379a6705fec24a2493fa68e011692605f44e119
    metrics:
    - type: accuracy
      value: 31.785999999999998
    - type: f1
      value: 31.40726949960717
  - task:
      type: Retrieval
    dataset:
      type: arguana
      name: MTEB ArguAna
      config: default
      split: test
      revision: 5b3e3697907184a9b77a3c99ee9ea1a9cbb1e4e3
    metrics:
    - type: map_at_1
      value: 25.605
    - type: map_at_10
      value: 41.165
    - type: map_at_100
      value: 42.230000000000004
    - type: map_at_1000
      value: 42.241
    - type: map_at_3
      value: 35.965
    - type: map_at_5
      value: 38.981
    - type: ndcg_at_1
      value: 25.605
    - type: ndcg_at_10
      value: 50.166999999999994
    - type: ndcg_at_100
      value: 54.534000000000006
    - type: ndcg_at_1000
      value: 54.772
    - type: ndcg_at_3
      value: 39.434000000000005
    - type: ndcg_at_5
      value: 44.876
    - type: precision_at_1
      value: 25.605
    - type: precision_at_10
      value: 7.908999999999999
    - type: precision_at_100
      value: 0.9769999999999999
    - type: precision_at_1000
      value: 0.1
    - type: precision_at_3
      value: 16.500999999999998
    - type: precision_at_5
      value: 12.546
    - type: recall_at_1
      value: 25.605
    - type: recall_at_10
      value: 79.09
    - type: recall_at_100
      value: 97.724
    - type: recall_at_1000
      value: 99.502
    - type: recall_at_3
      value: 49.502
    - type: recall_at_5
      value: 62.731
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-p2p
      name: MTEB ArxivClusteringP2P
      config: default
      split: test
      revision: 0bbdb47bcbe3a90093699aefeed338a0f28a7ee8
    metrics:
    - type: v_measure
      value: 46.54595079050156
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-s2s
      name: MTEB ArxivClusteringS2S
      config: default
      split: test
      revision: b73bd54100e5abfa6e3a23dcafb46fe4d2438dc3
    metrics:
    - type: v_measure
      value: 37.85709823840442
  - task:
      type: Reranking
    dataset:
      type: mteb/askubuntudupquestions-reranking
      name: MTEB AskUbuntuDupQuestions
      config: default
      split: test
      revision: 4d853f94cd57d85ec13805aeeac3ae3e5eb4c49c
    metrics:
    - type: map
      value: 63.47681681237331
    - type: mrr
      value: 77.08657608934617
  - task:
      type: STS
    dataset:
      type: mteb/biosses-sts
      name: MTEB BIOSSES
      config: default
      split: test
      revision: 9ee918f184421b6bd48b78f6c714d86546106103
    metrics:
    - type: cos_sim_pearson
      value: 84.41897516342782
    - type: cos_sim_spearman
      value: 81.64041444909368
    - type: euclidean_pearson
      value: 82.67500318274435
    - type: euclidean_spearman
      value: 81.64041444909368
    - type: manhattan_pearson
      value: 82.35165974372227
    - type: manhattan_spearman
      value: 81.50968857884978
  - task:
      type: Classification
    dataset:
      type: mteb/banking77
      name: MTEB Banking77Classification
      config: default
      split: test
      revision: 44fa15921b4c889113cc5df03dd4901b49161ab7
    metrics:
    - type: accuracy
      value: 79.75000000000001
    - type: f1
      value: 78.92604185699534
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-p2p
      name: MTEB BiorxivClusteringP2P
      config: default
      split: test
      revision: 11d0121201d1f1f280e8cc8f3d98fb9c4d9f9c55
    metrics:
    - type: v_measure
      value: 38.48301914135123
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-s2s
      name: MTEB BiorxivClusteringS2S
      config: default
      split: test
      revision: c0fab014e1bcb8d3a5e31b2088972a1e01547dc1
    metrics:
    - type: v_measure
      value: 33.170209943399804
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackAndroidRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 34.660000000000004
    - type: map_at_10
      value: 46.938
    - type: map_at_100
      value: 48.435
    - type: map_at_1000
      value: 48.555
    - type: map_at_3
      value: 43.034
    - type: map_at_5
      value: 45.055
    - type: ndcg_at_1
      value: 42.775
    - type: ndcg_at_10
      value: 53.82900000000001
    - type: ndcg_at_100
      value: 58.74700000000001
    - type: ndcg_at_1000
      value: 60.309000000000005
    - type: ndcg_at_3
      value: 48.487
    - type: ndcg_at_5
      value: 50.722
    - type: precision_at_1
      value: 42.775
    - type: precision_at_10
      value: 10.629
    - type: precision_at_100
      value: 1.652
    - type: precision_at_1000
      value: 0.209
    - type: precision_at_3
      value: 23.366999999999997
    - type: precision_at_5
      value: 16.967
    - type: recall_at_1
      value: 34.660000000000004
    - type: recall_at_10
      value: 66.465
    - type: recall_at_100
      value: 87.559
    - type: recall_at_1000
      value: 97.18299999999999
    - type: recall_at_3
      value: 51.01
    - type: recall_at_5
      value: 57.412
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackEnglishRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 31.180999999999997
    - type: map_at_10
      value: 41.802
    - type: map_at_100
      value: 43.294
    - type: map_at_1000
      value: 43.438
    - type: map_at_3
      value: 38.668
    - type: map_at_5
      value: 40.559
    - type: ndcg_at_1
      value: 39.489999999999995
    - type: ndcg_at_10
      value: 47.776
    - type: ndcg_at_100
      value: 52.705
    - type: ndcg_at_1000
      value: 54.830999999999996
    - type: ndcg_at_3
      value: 43.649
    - type: ndcg_at_5
      value: 45.885
    - type: precision_at_1
      value: 39.489999999999995
    - type: precision_at_10
      value: 9.121
    - type: precision_at_100
      value: 1.504
    - type: precision_at_1000
      value: 0.2
    - type: precision_at_3
      value: 21.38
    - type: precision_at_5
      value: 15.35
    - type: recall_at_1
      value: 31.180999999999997
    - type: recall_at_10
      value: 57.714
    - type: recall_at_100
      value: 78.342
    - type: recall_at_1000
      value: 91.586
    - type: recall_at_3
      value: 45.255
    - type: recall_at_5
      value: 51.459999999999994
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGamingRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 38.732
    - type: map_at_10
      value: 51.03
    - type: map_at_100
      value: 52.078
    - type: map_at_1000
      value: 52.132
    - type: map_at_3
      value: 47.735
    - type: map_at_5
      value: 49.562
    - type: ndcg_at_1
      value: 44.074999999999996
    - type: ndcg_at_10
      value: 56.923
    - type: ndcg_at_100
      value: 61.004999999999995
    - type: ndcg_at_1000
      value: 62.12800000000001
    - type: ndcg_at_3
      value: 51.381
    - type: ndcg_at_5
      value: 54.027
    - type: precision_at_1
      value: 44.074999999999996
    - type: precision_at_10
      value: 9.21
    - type: precision_at_100
      value: 1.221
    - type: precision_at_1000
      value: 0.136
    - type: precision_at_3
      value: 23.009
    - type: precision_at_5
      value: 15.748999999999999
    - type: recall_at_1
      value: 38.732
    - type: recall_at_10
      value: 71.154
    - type: recall_at_100
      value: 88.676
    - type: recall_at_1000
      value: 96.718
    - type: recall_at_3
      value: 56.288000000000004
    - type: recall_at_5
      value: 62.792
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGisRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 26.837
    - type: map_at_10
      value: 35.959
    - type: map_at_100
      value: 37.172
    - type: map_at_1000
      value: 37.241
    - type: map_at_3
      value: 33.027
    - type: map_at_5
      value: 34.699000000000005
    - type: ndcg_at_1
      value: 29.378999999999998
    - type: ndcg_at_10
      value: 41.31
    - type: ndcg_at_100
      value: 47.058
    - type: ndcg_at_1000
      value: 48.777
    - type: ndcg_at_3
      value: 35.564
    - type: ndcg_at_5
      value: 38.384
    - type: precision_at_1
      value: 29.378999999999998
    - type: precision_at_10
      value: 6.361999999999999
    - type: precision_at_100
      value: 0.98
    - type: precision_at_1000
      value: 0.117
    - type: precision_at_3
      value: 15.028
    - type: precision_at_5
      value: 10.667
    - type: recall_at_1
      value: 26.837
    - type: recall_at_10
      value: 55.667
    - type: recall_at_100
      value: 81.843
    - type: recall_at_1000
      value: 94.707
    - type: recall_at_3
      value: 40.049
    - type: recall_at_5
      value: 46.92
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackMathematicaRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 15.142
    - type: map_at_10
      value: 23.727999999999998
    - type: map_at_100
      value: 25.137999999999998
    - type: map_at_1000
      value: 25.256
    - type: map_at_3
      value: 20.673
    - type: map_at_5
      value: 22.325999999999997
    - type: ndcg_at_1
      value: 18.407999999999998
    - type: ndcg_at_10
      value: 29.286
    - type: ndcg_at_100
      value: 35.753
    - type: ndcg_at_1000
      value: 38.541
    - type: ndcg_at_3
      value: 23.599
    - type: ndcg_at_5
      value: 26.262
    - type: precision_at_1
      value: 18.407999999999998
    - type: precision_at_10
      value: 5.697
    - type: precision_at_100
      value: 1.034
    - type: precision_at_1000
      value: 0.14100000000000001
    - type: precision_at_3
      value: 11.567
    - type: precision_at_5
      value: 8.781
    - type: recall_at_1
      value: 15.142
    - type: recall_at_10
      value: 42.476
    - type: recall_at_100
      value: 70.22699999999999
    - type: recall_at_1000
      value: 90.02799999999999
    - type: recall_at_3
      value: 27.056
    - type: recall_at_5
      value: 33.663
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackPhysicsRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 29.142000000000003
    - type: map_at_10
      value: 40.735
    - type: map_at_100
      value: 42.155
    - type: map_at_1000
      value: 42.27
    - type: map_at_3
      value: 37.491
    - type: map_at_5
      value: 39.475
    - type: ndcg_at_1
      value: 35.515
    - type: ndcg_at_10
      value: 46.982
    - type: ndcg_at_100
      value: 52.913
    - type: ndcg_at_1000
      value: 54.759
    - type: ndcg_at_3
      value: 42.164
    - type: ndcg_at_5
      value: 44.674
    - type: precision_at_1
      value: 35.515
    - type: precision_at_10
      value: 8.624
    - type: precision_at_100
      value: 1.377
    - type: precision_at_1000
      value: 0.173
    - type: precision_at_3
      value: 20.468
    - type: precision_at_5
      value: 14.649000000000001
    - type: recall_at_1
      value: 29.142000000000003
    - type: recall_at_10
      value: 59.693
    - type: recall_at_100
      value: 84.84899999999999
    - type: recall_at_1000
      value: 96.451
    - type: recall_at_3
      value: 46.086
    - type: recall_at_5
      value: 52.556000000000004
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackProgrammersRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 22.081999999999997
    - type: map_at_10
      value: 32.74
    - type: map_at_100
      value: 34.108
    - type: map_at_1000
      value: 34.233000000000004
    - type: map_at_3
      value: 29.282999999999998
    - type: map_at_5
      value: 31.127
    - type: ndcg_at_1
      value: 26.712000000000003
    - type: ndcg_at_10
      value: 38.968
    - type: ndcg_at_100
      value: 44.64
    - type: ndcg_at_1000
      value: 47.193000000000005
    - type: ndcg_at_3
      value: 33.311
    - type: ndcg_at_5
      value: 35.76
    - type: precision_at_1
      value: 26.712000000000003
    - type: precision_at_10
      value: 7.534000000000001
    - type: precision_at_100
      value: 1.2149999999999999
    - type: precision_at_1000
      value: 0.163
    - type: precision_at_3
      value: 16.476
    - type: precision_at_5
      value: 12.009
    - type: recall_at_1
      value: 22.081999999999997
    - type: recall_at_10
      value: 52.859
    - type: recall_at_100
      value: 76.812
    - type: recall_at_1000
      value: 94.248
    - type: recall_at_3
      value: 36.964999999999996
    - type: recall_at_5
      value: 43.338
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 25.825750000000003
    - type: map_at_10
      value: 35.614666666666665
    - type: map_at_100
      value: 36.952416666666664
    - type: map_at_1000
      value: 37.07433333333334
    - type: map_at_3
      value: 32.519916666666674
    - type: map_at_5
      value: 34.22966666666667
    - type: ndcg_at_1
      value: 30.616416666666662
    - type: ndcg_at_10
      value: 41.32475
    - type: ndcg_at_100
      value: 46.907
    - type: ndcg_at_1000
      value: 49.12475
    - type: ndcg_at_3
      value: 36.1415
    - type: ndcg_at_5
      value: 38.54916666666666
    - type: precision_at_1
      value: 30.616416666666662
    - type: precision_at_10
      value: 7.427166666666666
    - type: precision_at_100
      value: 1.2174166666666666
    - type: precision_at_1000
      value: 0.16066666666666665
    - type: precision_at_3
      value: 16.849083333333333
    - type: precision_at_5
      value: 12.1105
    - type: recall_at_1
      value: 25.825750000000003
    - type: recall_at_10
      value: 53.95283333333333
    - type: recall_at_100
      value: 78.408
    - type: recall_at_1000
      value: 93.60841666666666
    - type: recall_at_3
      value: 39.51116666666667
    - type: recall_at_5
      value: 45.67041666666667
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackStatsRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 23.147000000000002
    - type: map_at_10
      value: 30.867
    - type: map_at_100
      value: 31.961000000000002
    - type: map_at_1000
      value: 32.074999999999996
    - type: map_at_3
      value: 28.598000000000003
    - type: map_at_5
      value: 29.715000000000003
    - type: ndcg_at_1
      value: 26.074
    - type: ndcg_at_10
      value: 35.379
    - type: ndcg_at_100
      value: 40.668
    - type: ndcg_at_1000
      value: 43.271
    - type: ndcg_at_3
      value: 31.291000000000004
    - type: ndcg_at_5
      value: 32.828
    - type: precision_at_1
      value: 26.074
    - type: precision_at_10
      value: 5.782
    - type: precision_at_100
      value: 0.9159999999999999
    - type: precision_at_1000
      value: 0.121
    - type: precision_at_3
      value: 13.905999999999999
    - type: precision_at_5
      value: 9.508999999999999
    - type: recall_at_1
      value: 23.147000000000002
    - type: recall_at_10
      value: 46.308
    - type: recall_at_100
      value: 70.529
    - type: recall_at_1000
      value: 89.53
    - type: recall_at_3
      value: 34.504000000000005
    - type: recall_at_5
      value: 38.472
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackTexRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 17.573
    - type: map_at_10
      value: 25.480999999999998
    - type: map_at_100
      value: 26.740000000000002
    - type: map_at_1000
      value: 26.881
    - type: map_at_3
      value: 22.962
    - type: map_at_5
      value: 24.366
    - type: ndcg_at_1
      value: 21.783
    - type: ndcg_at_10
      value: 30.519000000000002
    - type: ndcg_at_100
      value: 36.449
    - type: ndcg_at_1000
      value: 39.476
    - type: ndcg_at_3
      value: 26.104
    - type: ndcg_at_5
      value: 28.142
    - type: precision_at_1
      value: 21.783
    - type: precision_at_10
      value: 5.716
    - type: precision_at_100
      value: 1.036
    - type: precision_at_1000
      value: 0.149
    - type: precision_at_3
      value: 12.629000000000001
    - type: precision_at_5
      value: 9.188
    - type: recall_at_1
      value: 17.573
    - type: recall_at_10
      value: 41.565999999999995
    - type: recall_at_100
      value: 68.31099999999999
    - type: recall_at_1000
      value: 89.66
    - type: recall_at_3
      value: 28.998
    - type: recall_at_5
      value: 34.409
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackUnixRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 25.393
    - type: map_at_10
      value: 35.408
    - type: map_at_100
      value: 36.765
    - type: map_at_1000
      value: 36.870000000000005
    - type: map_at_3
      value: 31.858999999999998
    - type: map_at_5
      value: 34.088
    - type: ndcg_at_1
      value: 30.409999999999997
    - type: ndcg_at_10
      value: 41.31
    - type: ndcg_at_100
      value: 47.317
    - type: ndcg_at_1000
      value: 49.451
    - type: ndcg_at_3
      value: 35.156
    - type: ndcg_at_5
      value: 38.550000000000004
    - type: precision_at_1
      value: 30.409999999999997
    - type: precision_at_10
      value: 7.285
    - type: precision_at_100
      value: 1.16
    - type: precision_at_1000
      value: 0.145
    - type: precision_at_3
      value: 16.2
    - type: precision_at_5
      value: 12.015
    - type: recall_at_1
      value: 25.393
    - type: recall_at_10
      value: 54.955
    - type: recall_at_100
      value: 81.074
    - type: recall_at_1000
      value: 95.517
    - type: recall_at_3
      value: 38.646
    - type: recall_at_5
      value: 47.155
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWebmastersRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 25.219
    - type: map_at_10
      value: 34.317
    - type: map_at_100
      value: 36.099
    - type: map_at_1000
      value: 36.339
    - type: map_at_3
      value: 31.118000000000002
    - type: map_at_5
      value: 32.759
    - type: ndcg_at_1
      value: 30.04
    - type: ndcg_at_10
      value: 40.467
    - type: ndcg_at_100
      value: 46.918
    - type: ndcg_at_1000
      value: 49.263
    - type: ndcg_at_3
      value: 34.976
    - type: ndcg_at_5
      value: 37.345
    - type: precision_at_1
      value: 30.04
    - type: precision_at_10
      value: 7.786999999999999
    - type: precision_at_100
      value: 1.638
    - type: precision_at_1000
      value: 0.249
    - type: precision_at_3
      value: 16.206
    - type: precision_at_5
      value: 11.976
    - type: recall_at_1
      value: 25.219
    - type: recall_at_10
      value: 52.443
    - type: recall_at_100
      value: 80.523
    - type: recall_at_1000
      value: 95.025
    - type: recall_at_3
      value: 37.216
    - type: recall_at_5
      value: 43.086999999999996
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWordpressRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 20.801
    - type: map_at_10
      value: 28.371000000000002
    - type: map_at_100
      value: 29.483999999999998
    - type: map_at_1000
      value: 29.602
    - type: map_at_3
      value: 25.790999999999997
    - type: map_at_5
      value: 27.025
    - type: ndcg_at_1
      value: 22.736
    - type: ndcg_at_10
      value: 33.147999999999996
    - type: ndcg_at_100
      value: 38.711
    - type: ndcg_at_1000
      value: 41.498000000000005
    - type: ndcg_at_3
      value: 28.016000000000002
    - type: ndcg_at_5
      value: 30.011
    - type: precision_at_1
      value: 22.736
    - type: precision_at_10
      value: 5.379
    - type: precision_at_100
      value: 0.876
    - type: precision_at_1000
      value: 0.125
    - type: precision_at_3
      value: 11.953
    - type: precision_at_5
      value: 8.466
    - type: recall_at_1
      value: 20.801
    - type: recall_at_10
      value: 46.134
    - type: recall_at_100
      value: 72.151
    - type: recall_at_1000
      value: 92.648
    - type: recall_at_3
      value: 32.061
    - type: recall_at_5
      value: 36.781000000000006
  - task:
      type: Retrieval
    dataset:
      type: climate-fever
      name: MTEB ClimateFEVER
      config: default
      split: test
      revision: 392b78eb68c07badcd7c2cd8f39af108375dfcce
    metrics:
    - type: map_at_1
      value: 7.9159999999999995
    - type: map_at_10
      value: 13.769
    - type: map_at_100
      value: 15.447
    - type: map_at_1000
      value: 15.634
    - type: map_at_3
      value: 11.234
    - type: map_at_5
      value: 12.581999999999999
    - type: ndcg_at_1
      value: 17.72
    - type: ndcg_at_10
      value: 20.272000000000002
    - type: ndcg_at_100
      value: 27.748
    - type: ndcg_at_1000
      value: 31.457
    - type: ndcg_at_3
      value: 15.742
    - type: ndcg_at_5
      value: 17.494
    - type: precision_at_1
      value: 17.72
    - type: precision_at_10
      value: 6.554
    - type: precision_at_100
      value: 1.438
    - type: precision_at_1000
      value: 0.212
    - type: precision_at_3
      value: 11.705
    - type: precision_at_5
      value: 9.511
    - type: recall_at_1
      value: 7.9159999999999995
    - type: recall_at_10
      value: 25.389
    - type: recall_at_100
      value: 52.042
    - type: recall_at_1000
      value: 73.166
    - type: recall_at_3
      value: 14.585999999999999
    - type: recall_at_5
      value: 19.145
  - task:
      type: Retrieval
    dataset:
      type: dbpedia-entity
      name: MTEB DBPedia
      config: default
      split: test
      revision: f097057d03ed98220bc7309ddb10b71a54d667d6
    metrics:
    - type: map_at_1
      value: 7.172000000000001
    - type: map_at_10
      value: 14.507
    - type: map_at_100
      value: 20.094
    - type: map_at_1000
      value: 21.357
    - type: map_at_3
      value: 10.45
    - type: map_at_5
      value: 12.135
    - type: ndcg_at_1
      value: 42.375
    - type: ndcg_at_10
      value: 32.33
    - type: ndcg_at_100
      value: 36.370000000000005
    - type: ndcg_at_1000
      value: 43.596000000000004
    - type: ndcg_at_3
      value: 35.006
    - type: ndcg_at_5
      value: 33.35
    - type: precision_at_1
      value: 54.50000000000001
    - type: precision_at_10
      value: 26.424999999999997
    - type: precision_at_100
      value: 8.24
    - type: precision_at_1000
      value: 1.765
    - type: precision_at_3
      value: 38.667
    - type: precision_at_5
      value: 33.0
    - type: recall_at_1
      value: 7.172000000000001
    - type: recall_at_10
      value: 19.922
    - type: recall_at_100
      value: 43.273
    - type: recall_at_1000
      value: 67.157
    - type: recall_at_3
      value: 11.521
    - type: recall_at_5
      value: 14.667
  - task:
      type: Classification
    dataset:
      type: mteb/emotion
      name: MTEB EmotionClassification
      config: default
      split: test
      revision: 829147f8f75a25f005913200eb5ed41fae320aa1
    metrics:
    - type: accuracy
      value: 38.43
    - type: f1
      value: 35.26220518237799
  - task:
      type: Retrieval
    dataset:
      type: fever
      name: MTEB FEVER
      config: default
      split: test
      revision: 1429cf27e393599b8b359b9b72c666f96b2525f9
    metrics:
    - type: map_at_1
      value: 34.076
    - type: map_at_10
      value: 45.482
    - type: map_at_100
      value: 46.269
    - type: map_at_1000
      value: 46.309
    - type: map_at_3
      value: 42.614000000000004
    - type: map_at_5
      value: 44.314
    - type: ndcg_at_1
      value: 36.529
    - type: ndcg_at_10
      value: 51.934000000000005
    - type: ndcg_at_100
      value: 55.525000000000006
    - type: ndcg_at_1000
      value: 56.568
    - type: ndcg_at_3
      value: 46.169
    - type: ndcg_at_5
      value: 49.163000000000004
    - type: precision_at_1
      value: 36.529
    - type: precision_at_10
      value: 7.5649999999999995
    - type: precision_at_100
      value: 0.947
    - type: precision_at_1000
      value: 0.105
    - type: precision_at_3
      value: 19.326999999999998
    - type: precision_at_5
      value: 13.239999999999998
    - type: recall_at_1
      value: 34.076
    - type: recall_at_10
      value: 69.009
    - type: recall_at_100
      value: 85.047
    - type: recall_at_1000
      value: 92.962
    - type: recall_at_3
      value: 53.446000000000005
    - type: recall_at_5
      value: 60.622
  - task:
      type: Retrieval
    dataset:
      type: fiqa
      name: MTEB FiQA2018
      config: default
      split: test
      revision: 41b686a7f28c59bcaaa5791efd47c67c8ebe28be
    metrics:
    - type: map_at_1
      value: 17.14
    - type: map_at_10
      value: 29.141000000000002
    - type: map_at_100
      value: 30.956
    - type: map_at_1000
      value: 31.159
    - type: map_at_3
      value: 25.188
    - type: map_at_5
      value: 27.506999999999998
    - type: ndcg_at_1
      value: 34.721999999999994
    - type: ndcg_at_10
      value: 36.867
    - type: ndcg_at_100
      value: 43.931
    - type: ndcg_at_1000
      value: 47.276
    - type: ndcg_at_3
      value: 33.18
    - type: ndcg_at_5
      value: 34.504000000000005
    - type: precision_at_1
      value: 34.721999999999994
    - type: precision_at_10
      value: 10.448
    - type: precision_at_100
      value: 1.778
    - type: precision_at_1000
      value: 0.23600000000000002
    - type: precision_at_3
      value: 22.377
    - type: precision_at_5
      value: 16.759
    - type: recall_at_1
      value: 17.14
    - type: recall_at_10
      value: 44.131
    - type: recall_at_100
      value: 70.60600000000001
    - type: recall_at_1000
      value: 90.672
    - type: recall_at_3
      value: 30.536
    - type: recall_at_5
      value: 36.706
  - task:
      type: Retrieval
    dataset:
      type: hotpotqa
      name: MTEB HotpotQA
      config: default
      split: test
      revision: 766870b35a1b9ca65e67a0d1913899973551fc6c
    metrics:
    - type: map_at_1
      value: 27.717999999999996
    - type: map_at_10
      value: 37.63
    - type: map_at_100
      value: 38.534
    - type: map_at_1000
      value: 38.619
    - type: map_at_3
      value: 35.197
    - type: map_at_5
      value: 36.592999999999996
    - type: ndcg_at_1
      value: 55.43599999999999
    - type: ndcg_at_10
      value: 46.513
    - type: ndcg_at_100
      value: 50.21
    - type: ndcg_at_1000
      value: 52.049
    - type: ndcg_at_3
      value: 42.333999999999996
    - type: ndcg_at_5
      value: 44.45
    - type: precision_at_1
      value: 55.43599999999999
    - type: precision_at_10
      value: 9.741
    - type: precision_at_100
      value: 1.2670000000000001
    - type: precision_at_1000
      value: 0.151
    - type: precision_at_3
      value: 26.194
    - type: precision_at_5
      value: 17.396
    - type: recall_at_1
      value: 27.717999999999996
    - type: recall_at_10
      value: 48.704
    - type: recall_at_100
      value: 63.363
    - type: recall_at_1000
      value: 75.564
    - type: recall_at_3
      value: 39.291
    - type: recall_at_5
      value: 43.491
  - task:
      type: Classification
    dataset:
      type: mteb/imdb
      name: MTEB ImdbClassification
      config: default
      split: test
      revision: 8d743909f834c38949e8323a8a6ce8721ea6c7f4
    metrics:
    - type: accuracy
      value: 60.6612
    - type: ap
      value: 56.73559487964456
    - type: f1
      value: 60.39970244353384
  - task:
      type: Retrieval
    dataset:
      type: msmarco
      name: MTEB MSMARCO
      config: default
      split: dev
      revision: e6838a846e2408f22cf5cc337ebc83e0bcf77849
    metrics:
    - type: map_at_1
      value: 18.715
    - type: map_at_10
      value: 30.014999999999997
    - type: map_at_100
      value: 31.208999999999996
    - type: map_at_1000
      value: 31.269999999999996
    - type: map_at_3
      value: 26.299
    - type: map_at_5
      value: 28.408
    - type: ndcg_at_1
      value: 19.255
    - type: ndcg_at_10
      value: 36.542
    - type: ndcg_at_100
      value: 42.471
    - type: ndcg_at_1000
      value: 44.022
    - type: ndcg_at_3
      value: 28.921000000000003
    - type: ndcg_at_5
      value: 32.676
    - type: precision_at_1
      value: 19.255
    - type: precision_at_10
      value: 5.91
    - type: precision_at_100
      value: 0.8920000000000001
    - type: precision_at_1000
      value: 0.10200000000000001
    - type: precision_at_3
      value: 12.388
    - type: precision_at_5
      value: 9.33
    - type: recall_at_1
      value: 18.715
    - type: recall_at_10
      value: 56.76
    - type: recall_at_100
      value: 84.481
    - type: recall_at_1000
      value: 96.44
    - type: recall_at_3
      value: 35.942
    - type: recall_at_5
      value: 44.926
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (en)
      config: en
      split: test
      revision: a7e2a951126a26fc8c6a69f835f33a346ba259e3
    metrics:
    - type: accuracy
      value: 91.56178750569997
    - type: f1
      value: 91.02309252160694
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (en)
      config: en
      split: test
      revision: 6299947a7777084cc2d4b64235bf7190381ce755
    metrics:
    - type: accuracy
      value: 62.18194254445966
    - type: f1
      value: 43.090624769020444
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (en)
      config: en
      split: test
      revision: 072a486a144adf7f4479a4a0dddb2152e161e1ea
    metrics:
    - type: accuracy
      value: 67.404169468729
    - type: f1
      value: 64.82901615433794
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (en)
      config: en
      split: test
      revision: 7d571f92784cd94a019292a1f45445077d0ef634
    metrics:
    - type: accuracy
      value: 75.75655682582381
    - type: f1
      value: 74.93126114560368
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-p2p
      name: MTEB MedrxivClusteringP2P
      config: default
      split: test
      revision: dcefc037ef84348e49b0d29109e891c01067226b
    metrics:
    - type: v_measure
      value: 34.40873490143895
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-s2s
      name: MTEB MedrxivClusteringS2S
      config: default
      split: test
      revision: 3cd0e71dfbe09d4de0f9e5ecba43e7ce280959dc
    metrics:
    - type: v_measure
      value: 32.292207500530914
  - task:
      type: Reranking
    dataset:
      type: mteb/mind_small
      name: MTEB MindSmallReranking
      config: default
      split: test
      revision: 3bdac13927fdc888b903db93b2ffdbd90b295a69
    metrics:
    - type: map
      value: 30.798042020200267
    - type: mrr
      value: 31.803264263405513
  - task:
      type: Retrieval
    dataset:
      type: nfcorpus
      name: MTEB NFCorpus
      config: default
      split: test
      revision: 7eb63cc0c1eb59324d709ebed25fcab851fa7610
    metrics:
    - type: map_at_1
      value: 4.3229999999999995
    - type: map_at_10
      value: 11.048
    - type: map_at_100
      value: 14.244000000000002
    - type: map_at_1000
      value: 15.684000000000001
    - type: map_at_3
      value: 7.7219999999999995
    - type: map_at_5
      value: 9.231
    - type: ndcg_at_1
      value: 39.474
    - type: ndcg_at_10
      value: 31.594
    - type: ndcg_at_100
      value: 29.455
    - type: ndcg_at_1000
      value: 38.283
    - type: ndcg_at_3
      value: 36.355
    - type: ndcg_at_5
      value: 34.164
    - type: precision_at_1
      value: 41.486000000000004
    - type: precision_at_10
      value: 24.334
    - type: precision_at_100
      value: 7.981000000000001
    - type: precision_at_1000
      value: 2.096
    - type: precision_at_3
      value: 34.881
    - type: precision_at_5
      value: 30.279
    - type: recall_at_1
      value: 4.3229999999999995
    - type: recall_at_10
      value: 15.498999999999999
    - type: recall_at_100
      value: 31.151
    - type: recall_at_1000
      value: 63.211
    - type: recall_at_3
      value: 9.053
    - type: recall_at_5
      value: 11.959
  - task:
      type: Retrieval
    dataset:
      type: nq
      name: MTEB NQ
      config: default
      split: test
      revision: 6062aefc120bfe8ece5897809fb2e53bfe0d128c
    metrics:
    - type: map_at_1
      value: 22.644000000000002
    - type: map_at_10
      value: 36.335
    - type: map_at_100
      value: 37.687
    - type: map_at_1000
      value: 37.733
    - type: map_at_3
      value: 31.928
    - type: map_at_5
      value: 34.586
    - type: ndcg_at_1
      value: 25.607999999999997
    - type: ndcg_at_10
      value: 43.869
    - type: ndcg_at_100
      value: 49.730000000000004
    - type: ndcg_at_1000
      value: 50.749
    - type: ndcg_at_3
      value: 35.418
    - type: ndcg_at_5
      value: 39.961999999999996
    - type: precision_at_1
      value: 25.607999999999997
    - type: precision_at_10
      value: 7.697
    - type: precision_at_100
      value: 1.093
    - type: precision_at_1000
      value: 0.11900000000000001
    - type: precision_at_3
      value: 16.522000000000002
    - type: precision_at_5
      value: 12.486
    - type: recall_at_1
      value: 22.644000000000002
    - type: recall_at_10
      value: 64.711
    - type: recall_at_100
      value: 90.32900000000001
    - type: recall_at_1000
      value: 97.82
    - type: recall_at_3
      value: 42.754999999999995
    - type: recall_at_5
      value: 53.37
  - task:
      type: Retrieval
    dataset:
      type: quora
      name: MTEB QuoraRetrieval
      config: default
      split: test
      revision: 6205996560df11e3a3da9ab4f926788fc30a7db4
    metrics:
    - type: map_at_1
      value: 69.76
    - type: map_at_10
      value: 83.64200000000001
    - type: map_at_100
      value: 84.312
    - type: map_at_1000
      value: 84.329
    - type: map_at_3
      value: 80.537
    - type: map_at_5
      value: 82.494
    - type: ndcg_at_1
      value: 80.41
    - type: ndcg_at_10
      value: 87.556
    - type: ndcg_at_100
      value: 88.847
    - type: ndcg_at_1000
      value: 88.959
    - type: ndcg_at_3
      value: 84.466
    - type: ndcg_at_5
      value: 86.193
    - type: precision_at_1
      value: 80.41
    - type: precision_at_10
      value: 13.374
    - type: precision_at_100
      value: 1.529
    - type: precision_at_1000
      value: 0.157
    - type: precision_at_3
      value: 36.953
    - type: precision_at_5
      value: 24.401999999999997
    - type: recall_at_1
      value: 69.76
    - type: recall_at_10
      value: 95.029
    - type: recall_at_100
      value: 99.44
    - type: recall_at_1000
      value: 99.979
    - type: recall_at_3
      value: 86.215
    - type: recall_at_5
      value: 91.03999999999999
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering
      name: MTEB RedditClustering
      config: default
      split: test
      revision: b2805658ae38990172679479369a78b86de8c390
    metrics:
    - type: v_measure
      value: 50.66969274980475
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering-p2p
      name: MTEB RedditClusteringP2P
      config: default
      split: test
      revision: 385e3cb46b4cfa89021f56c4380204149d0efe33
    metrics:
    - type: v_measure
      value: 54.15176409632201
  - task:
      type: Retrieval
    dataset:
      type: scidocs
      name: MTEB SCIDOCS
      config: default
      split: test
      revision: 5c59ef3e437a0a9651c8fe6fde943e7dce59fba5
    metrics:
    - type: map_at_1
      value: 4.853
    - type: map_at_10
      value: 12.937999999999999
    - type: map_at_100
      value: 15.588
    - type: map_at_1000
      value: 15.939
    - type: map_at_3
      value: 9.135
    - type: map_at_5
      value: 11.004
    - type: ndcg_at_1
      value: 24.0
    - type: ndcg_at_10
      value: 21.641
    - type: ndcg_at_100
      value: 31.212
    - type: ndcg_at_1000
      value: 36.854
    - type: ndcg_at_3
      value: 20.284
    - type: ndcg_at_5
      value: 17.737
    - type: precision_at_1
      value: 24.0
    - type: precision_at_10
      value: 11.4
    - type: precision_at_100
      value: 2.516
    - type: precision_at_1000
      value: 0.387
    - type: precision_at_3
      value: 19.167
    - type: precision_at_5
      value: 15.72
    - type: recall_at_1
      value: 4.853
    - type: recall_at_10
      value: 23.087
    - type: recall_at_100
      value: 51.012
    - type: recall_at_1000
      value: 78.49000000000001
    - type: recall_at_3
      value: 11.658
    - type: recall_at_5
      value: 15.923000000000002
  - task:
      type: STS
    dataset:
      type: mteb/sickr-sts
      name: MTEB SICK-R
      config: default
      split: test
      revision: 20a6d6f312dd54037fe07a32d58e5e168867909d
    metrics:
    - type: cos_sim_pearson
      value: 83.91595834747078
    - type: cos_sim_spearman
      value: 77.58245130495686
    - type: euclidean_pearson
      value: 80.77605511224702
    - type: euclidean_spearman
      value: 77.58244681255565
    - type: manhattan_pearson
      value: 80.70675261518134
    - type: manhattan_spearman
      value: 77.48238642250558
  - task:
      type: STS
    dataset:
      type: mteb/sts12-sts
      name: MTEB STS12
      config: default
      split: test
      revision: fdf84275bb8ce4b49c971d02e84dd1abc677a50f
    metrics:
    - type: cos_sim_pearson
      value: 81.35998585185463
    - type: cos_sim_spearman
      value: 72.36900735029991
    - type: euclidean_pearson
      value: 77.44425972881783
    - type: euclidean_spearman
      value: 72.36900735029991
    - type: manhattan_pearson
      value: 77.48268272405316
    - type: manhattan_spearman
      value: 72.36650357806357
  - task:
      type: STS
    dataset:
      type: mteb/sts13-sts
      name: MTEB STS13
      config: default
      split: test
      revision: 1591bfcbe8c69d4bf7fe2a16e2451017832cafb9
    metrics:
    - type: cos_sim_pearson
      value: 80.15192226911441
    - type: cos_sim_spearman
      value: 80.60316722220763
    - type: euclidean_pearson
      value: 79.9515074804673
    - type: euclidean_spearman
      value: 80.60316715056034
    - type: manhattan_pearson
      value: 80.01037050043855
    - type: manhattan_spearman
      value: 80.70244228209006
  - task:
      type: STS
    dataset:
      type: mteb/sts14-sts
      name: MTEB STS14
      config: default
      split: test
      revision: e2125984e7df8b7871f6ae9949cf6b6795e7c54b
    metrics:
    - type: cos_sim_pearson
      value: 80.80137749134273
    - type: cos_sim_spearman
      value: 75.58912800301661
    - type: euclidean_pearson
      value: 78.89739732785547
    - type: euclidean_spearman
      value: 75.58912800301661
    - type: manhattan_pearson
      value: 78.88130916509184
    - type: manhattan_spearman
      value: 75.56512617108156
  - task:
      type: STS
    dataset:
      type: mteb/sts15-sts
      name: MTEB STS15
      config: default
      split: test
      revision: 1cd7298cac12a96a373b6a2f18738bb3e739a9b6
    metrics:
    - type: cos_sim_pearson
      value: 84.73605558012511
    - type: cos_sim_spearman
      value: 85.38966051883823
    - type: euclidean_pearson
      value: 84.65792305262497
    - type: euclidean_spearman
      value: 85.38965068015148
    - type: manhattan_pearson
      value: 84.6284531553976
    - type: manhattan_spearman
      value: 85.36525580485275
  - task:
      type: STS
    dataset:
      type: mteb/sts16-sts
      name: MTEB STS16
      config: default
      split: test
      revision: 360a0b2dff98700d09e634a01e1cc1624d3e42cd
    metrics:
    - type: cos_sim_pearson
      value: 77.93667023468089
    - type: cos_sim_spearman
      value: 78.98945343973261
    - type: euclidean_pearson
      value: 78.55627105899589
    - type: euclidean_spearman
      value: 78.98945343973261
    - type: manhattan_pearson
      value: 78.47171138630095
    - type: manhattan_spearman
      value: 78.90029153062082
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (ko-ko)
      config: ko-ko
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 38.02556869388448
    - type: cos_sim_spearman
      value: 43.39452386216687
    - type: euclidean_pearson
      value: 42.85346056221848
    - type: euclidean_spearman
      value: 43.39454482701475
    - type: manhattan_pearson
      value: 42.80255086270408
    - type: manhattan_spearman
      value: 43.35745739810561
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (ar-ar)
      config: ar-ar
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 50.19733275252325
    - type: cos_sim_spearman
      value: 50.892912699226166
    - type: euclidean_pearson
      value: 53.38352259940662
    - type: euclidean_spearman
      value: 50.892912699226166
    - type: manhattan_pearson
      value: 53.48429031763742
    - type: manhattan_spearman
      value: 50.961509277559394
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-ar)
      config: en-ar
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: -5.346248828225636
    - type: cos_sim_spearman
      value: -4.276245759627542
    - type: euclidean_pearson
      value: -5.34997238478067
    - type: euclidean_spearman
      value: -4.276245759627542
    - type: manhattan_pearson
      value: -1.599674226848396
    - type: manhattan_spearman
      value: -0.6972996366546237
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-de)
      config: en-de
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 37.0025013483991
    - type: cos_sim_spearman
      value: 35.81883942216964
    - type: euclidean_pearson
      value: 36.69612954510884
    - type: euclidean_spearman
      value: 35.81883942216964
    - type: manhattan_pearson
      value: 35.141229073611555
    - type: manhattan_spearman
      value: 32.04594883372404
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-en)
      config: en-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 88.02366672243191
    - type: cos_sim_spearman
      value: 87.58779089494524
    - type: euclidean_pearson
      value: 87.99011173645361
    - type: euclidean_spearman
      value: 87.58779089494524
    - type: manhattan_pearson
      value: 87.71266341564564
    - type: manhattan_spearman
      value: 87.24437101621581
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-tr)
      config: en-tr
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 6.928208810824121
    - type: cos_sim_spearman
      value: 4.496540073637865
    - type: euclidean_pearson
      value: 7.258004484570359
    - type: euclidean_spearman
      value: 4.496540073637865
    - type: manhattan_pearson
      value: 4.294687250993676
    - type: manhattan_spearman
      value: 2.517822531443102
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (es-en)
      config: es-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 17.49363358339176
    - type: cos_sim_spearman
      value: 16.31316318682868
    - type: euclidean_pearson
      value: 17.834234153786475
    - type: euclidean_spearman
      value: 16.31316318682868
    - type: manhattan_pearson
      value: 16.928139101229352
    - type: manhattan_spearman
      value: 15.00071366769135
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (es-es)
      config: es-es
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 77.04145671005833
    - type: cos_sim_spearman
      value: 76.11599994398748
    - type: euclidean_pearson
      value: 78.21801117699432
    - type: euclidean_spearman
      value: 76.11599994398748
    - type: manhattan_pearson
      value: 77.87062358292948
    - type: manhattan_spearman
      value: 75.64561332109221
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (fr-en)
      config: fr-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 37.9961687967439
    - type: cos_sim_spearman
      value: 37.09338306656542
    - type: euclidean_pearson
      value: 37.81002317191932
    - type: euclidean_spearman
      value: 37.09338306656542
    - type: manhattan_pearson
      value: 37.58237523973875
    - type: manhattan_spearman
      value: 36.52020936925911
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (it-en)
      config: it-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 26.739991134614716
    - type: cos_sim_spearman
      value: 24.4457755448559
    - type: euclidean_pearson
      value: 26.804935356831862
    - type: euclidean_spearman
      value: 24.442532087041023
    - type: manhattan_pearson
      value: 27.571123840765026
    - type: manhattan_spearman
      value: 25.554721155049045
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (nl-en)
      config: nl-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 32.71761762628939
    - type: cos_sim_spearman
      value: 28.99879893370601
    - type: euclidean_pearson
      value: 32.92831060810701
    - type: euclidean_spearman
      value: 28.99879893370601
    - type: manhattan_pearson
      value: 33.30410551798337
    - type: manhattan_spearman
      value: 29.442853829506593
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (en)
      config: en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 67.09882753030891
    - type: cos_sim_spearman
      value: 67.21465212910987
    - type: euclidean_pearson
      value: 68.21374069918403
    - type: euclidean_spearman
      value: 67.21465212910987
    - type: manhattan_pearson
      value: 68.41388868877884
    - type: manhattan_spearman
      value: 67.83615682571867
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de)
      config: de
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 26.596033966146116
    - type: cos_sim_spearman
      value: 31.044353994772354
    - type: euclidean_pearson
      value: 21.51728902500591
    - type: euclidean_spearman
      value: 31.044353994772354
    - type: manhattan_pearson
      value: 21.718468273577894
    - type: manhattan_spearman
      value: 31.197915595597696
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es)
      config: es
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 44.33815143022264
    - type: cos_sim_spearman
      value: 54.77772552456677
    - type: euclidean_pearson
      value: 48.483578263920634
    - type: euclidean_spearman
      value: 54.77772552456677
    - type: manhattan_pearson
      value: 49.29424073081744
    - type: manhattan_spearman
      value: 55.259696552690954
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (pl)
      config: pl
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 8.000336595206134
    - type: cos_sim_spearman
      value: 26.768906191975933
    - type: euclidean_pearson
      value: 1.4181188576056134
    - type: euclidean_spearman
      value: 26.768906191975933
    - type: manhattan_pearson
      value: 1.588769366202155
    - type: manhattan_spearman
      value: 26.76300987426348
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (tr)
      config: tr
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 20.597902459466386
    - type: cos_sim_spearman
      value: 33.694510807738595
    - type: euclidean_pearson
      value: 26.964862787540962
    - type: euclidean_spearman
      value: 33.694510807738595
    - type: manhattan_pearson
      value: 27.530294926210807
    - type: manhattan_spearman
      value: 33.74254435313719
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (ar)
      config: ar
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 5.006610360999117
    - type: cos_sim_spearman
      value: 22.63866797712348
    - type: euclidean_pearson
      value: 13.082283087945362
    - type: euclidean_spearman
      value: 22.63866797712348
    - type: manhattan_pearson
      value: 13.260328120447722
    - type: manhattan_spearman
      value: 22.340169287120716
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (ru)
      config: ru
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 0.03100716792233671
    - type: cos_sim_spearman
      value: 14.721380413194854
    - type: euclidean_pearson
      value: 4.871526064730011
    - type: euclidean_spearman
      value: 14.721380413194854
    - type: manhattan_pearson
      value: 5.7576102223040735
    - type: manhattan_spearman
      value: 15.08182690716095
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (zh)
      config: zh
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 23.127885111414432
    - type: cos_sim_spearman
      value: 44.92964024177277
    - type: euclidean_pearson
      value: 31.061639313469925
    - type: euclidean_spearman
      value: 44.92964024177277
    - type: manhattan_pearson
      value: 31.77656358573927
    - type: manhattan_spearman
      value: 44.964763982886375
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (fr)
      config: fr
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 70.64344773137496
    - type: cos_sim_spearman
      value: 77.00398643056744
    - type: euclidean_pearson
      value: 71.58320199923101
    - type: euclidean_spearman
      value: 77.00398643056744
    - type: manhattan_pearson
      value: 71.64373853764818
    - type: manhattan_spearman
      value: 76.71158725879226
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-en)
      config: de-en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 47.54531236654512
    - type: cos_sim_spearman
      value: 44.038685024247606
    - type: euclidean_pearson
      value: 48.46975590869453
    - type: euclidean_spearman
      value: 44.038685024247606
    - type: manhattan_pearson
      value: 48.10217367438755
    - type: manhattan_spearman
      value: 44.4428504653391
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es-en)
      config: es-en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 49.93601240112664
    - type: cos_sim_spearman
      value: 53.41895837272506
    - type: euclidean_pearson
      value: 50.16469746986203
    - type: euclidean_spearman
      value: 53.41895837272506
    - type: manhattan_pearson
      value: 49.86265183075983
    - type: manhattan_spearman
      value: 53.10065931046005
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (it)
      config: it
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 57.4312835830767
    - type: cos_sim_spearman
      value: 60.39610834515271
    - type: euclidean_pearson
      value: 57.81507077373551
    - type: euclidean_spearman
      value: 60.39610834515271
    - type: manhattan_pearson
      value: 57.83823485037898
    - type: manhattan_spearman
      value: 60.374938260317535
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (pl-en)
      config: pl-en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 35.08730015173829
    - type: cos_sim_spearman
      value: 32.79791295777814
    - type: euclidean_pearson
      value: 34.54132550386404
    - type: euclidean_spearman
      value: 32.79791295777814
    - type: manhattan_pearson
      value: 36.273935331272256
    - type: manhattan_spearman
      value: 35.88704294252439
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (zh-en)
      config: zh-en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 37.41111741585122
    - type: cos_sim_spearman
      value: 41.64399741744448
    - type: euclidean_pearson
      value: 36.83160927711053
    - type: euclidean_spearman
      value: 41.64399741744448
    - type: manhattan_pearson
      value: 35.71015224548175
    - type: manhattan_spearman
      value: 41.460551673456045
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es-it)
      config: es-it
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 42.568537775842245
    - type: cos_sim_spearman
      value: 44.2699366594503
    - type: euclidean_pearson
      value: 43.569828137034264
    - type: euclidean_spearman
      value: 44.2699366594503
    - type: manhattan_pearson
      value: 43.954212787242284
    - type: manhattan_spearman
      value: 44.32159550471527
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-fr)
      config: de-fr
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 26.472844763068938
    - type: cos_sim_spearman
      value: 30.067587482078228
    - type: euclidean_pearson
      value: 26.87230792075073
    - type: euclidean_spearman
      value: 30.067587482078228
    - type: manhattan_pearson
      value: 25.808959063835424
    - type: manhattan_spearman
      value: 27.996294873002153
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-pl)
      config: de-pl
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 7.026566971631159
    - type: cos_sim_spearman
      value: 4.9270565599404135
    - type: euclidean_pearson
      value: 6.729027056926625
    - type: euclidean_spearman
      value: 4.9270565599404135
    - type: manhattan_pearson
      value: 9.01762174854638
    - type: manhattan_spearman
      value: 7.359790736410993
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (fr-pl)
      config: fr-pl
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 54.305559003968206
    - type: cos_sim_spearman
      value: 50.709255283710995
    - type: euclidean_pearson
      value: 53.00660084455784
    - type: euclidean_spearman
      value: 50.709255283710995
    - type: manhattan_pearson
      value: 52.33784187543789
    - type: manhattan_spearman
      value: 50.709255283710995
  - task:
      type: STS
    dataset:
      type: mteb/stsbenchmark-sts
      name: MTEB STSBenchmark
      config: default
      split: test
      revision: 8913289635987208e6e7c72789e4be2fe94b6abd
    metrics:
    - type: cos_sim_pearson
      value: 82.7406424090513
    - type: cos_sim_spearman
      value: 82.03246731235654
    - type: euclidean_pearson
      value: 82.55616747173353
    - type: euclidean_spearman
      value: 82.03246731235654
    - type: manhattan_pearson
      value: 82.49144455072748
    - type: manhattan_spearman
      value: 81.94552526855261
  - task:
      type: Reranking
    dataset:
      type: mteb/scidocs-reranking
      name: MTEB SciDocsRR
      config: default
      split: test
      revision: 56a6d0140cf6356659e2a7c1413286a774468d44
    metrics:
    - type: map
      value: 87.11941318470207
    - type: mrr
      value: 96.39370705547176
  - task:
      type: Retrieval
    dataset:
      type: scifact
      name: MTEB SciFact
      config: default
      split: test
      revision: a75ae049398addde9b70f6b268875f5cbce99089
    metrics:
    - type: map_at_1
      value: 48.233
    - type: map_at_10
      value: 59.592999999999996
    - type: map_at_100
      value: 60.307
    - type: map_at_1000
      value: 60.343
    - type: map_at_3
      value: 56.564
    - type: map_at_5
      value: 58.826
    - type: ndcg_at_1
      value: 50.333000000000006
    - type: ndcg_at_10
      value: 64.508
    - type: ndcg_at_100
      value: 67.66499999999999
    - type: ndcg_at_1000
      value: 68.552
    - type: ndcg_at_3
      value: 59.673
    - type: ndcg_at_5
      value: 62.928
    - type: precision_at_1
      value: 50.333000000000006
    - type: precision_at_10
      value: 8.833
    - type: precision_at_100
      value: 1.053
    - type: precision_at_1000
      value: 0.11199999999999999
    - type: precision_at_3
      value: 23.778
    - type: precision_at_5
      value: 16.400000000000002
    - type: recall_at_1
      value: 48.233
    - type: recall_at_10
      value: 78.333
    - type: recall_at_100
      value: 92.5
    - type: recall_at_1000
      value: 99.333
    - type: recall_at_3
      value: 66.033
    - type: recall_at_5
      value: 73.79400000000001
  - task:
      type: PairClassification
    dataset:
      type: mteb/sprintduplicatequestions-pairclassification
      name: MTEB SprintDuplicateQuestions
      config: default
      split: test
      revision: 5a8256d0dff9c4bd3be3ba3e67e4e70173f802ea
    metrics:
    - type: cos_sim_accuracy
      value: 99.78514851485149
    - type: cos_sim_ap
      value: 94.55063045792446
    - type: cos_sim_f1
      value: 89.01265822784809
    - type: cos_sim_precision
      value: 90.15384615384615
    - type: cos_sim_recall
      value: 87.9
    - type: dot_accuracy
      value: 99.78514851485149
    - type: dot_ap
      value: 94.55063045792447
    - type: dot_f1
      value: 89.01265822784809
    - type: dot_precision
      value: 90.15384615384615
    - type: dot_recall
      value: 87.9
    - type: euclidean_accuracy
      value: 99.78514851485149
    - type: euclidean_ap
      value: 94.55063045792447
    - type: euclidean_f1
      value: 89.01265822784809
    - type: euclidean_precision
      value: 90.15384615384615
    - type: euclidean_recall
      value: 87.9
    - type: manhattan_accuracy
      value: 99.78415841584159
    - type: manhattan_ap
      value: 94.54002074215008
    - type: manhattan_f1
      value: 88.98989898989899
    - type: manhattan_precision
      value: 89.89795918367346
    - type: manhattan_recall
      value: 88.1
    - type: max_accuracy
      value: 99.78514851485149
    - type: max_ap
      value: 94.55063045792447
    - type: max_f1
      value: 89.01265822784809
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering
      name: MTEB StackExchangeClustering
      config: default
      split: test
      revision: 70a89468f6dccacc6aa2b12a6eac54e74328f235
    metrics:
    - type: v_measure
      value: 53.361421662036015
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering-p2p
      name: MTEB StackExchangeClusteringP2P
      config: default
      split: test
      revision: d88009ab563dd0b16cfaf4436abaf97fa3550cf0
    metrics:
    - type: v_measure
      value: 38.001825627800976
  - task:
      type: Reranking
    dataset:
      type: mteb/stackoverflowdupquestions-reranking
      name: MTEB StackOverflowDupQuestions
      config: default
      split: test
      revision: ef807ea29a75ec4f91b50fd4191cb4ee4589a9f9
    metrics:
    - type: map
      value: 50.762134384316084
    - type: mrr
      value: 51.39383594346829
  - task:
      type: Summarization
    dataset:
      type: mteb/summeval
      name: MTEB SummEval
      config: default
      split: test
      revision: 8753c2788d36c01fc6f05d03fe3f7268d63f9122
    metrics:
    - type: cos_sim_pearson
      value: 30.508420334813536
    - type: cos_sim_spearman
      value: 30.808757671244493
    - type: dot_pearson
      value: 30.508418240633862
    - type: dot_spearman
      value: 30.808757671244493
  - task:
      type: Retrieval
    dataset:
      type: trec-covid
      name: MTEB TRECCOVID
      config: default
      split: test
      revision: 2c8041b2c07a79b6f7ba8fe6acc72e5d9f92d217
    metrics:
    - type: map_at_1
      value: 0.169
    - type: map_at_10
      value: 1.054
    - type: map_at_100
      value: 5.308
    - type: map_at_1000
      value: 13.313
    - type: map_at_3
      value: 0.40800000000000003
    - type: map_at_5
      value: 0.627
    - type: ndcg_at_1
      value: 56.00000000000001
    - type: ndcg_at_10
      value: 47.246
    - type: ndcg_at_100
      value: 35.172
    - type: ndcg_at_1000
      value: 34.031
    - type: ndcg_at_3
      value: 51.939
    - type: ndcg_at_5
      value: 50.568999999999996
    - type: precision_at_1
      value: 62.0
    - type: precision_at_10
      value: 50.4
    - type: precision_at_100
      value: 36.14
    - type: precision_at_1000
      value: 15.45
    - type: precision_at_3
      value: 56.00000000000001
    - type: precision_at_5
      value: 55.2
    - type: recall_at_1
      value: 0.169
    - type: recall_at_10
      value: 1.284
    - type: recall_at_100
      value: 8.552
    - type: recall_at_1000
      value: 32.81
    - type: recall_at_3
      value: 0.44
    - type: recall_at_5
      value: 0.709
  - task:
      type: Retrieval
    dataset:
      type: webis-touche2020
      name: MTEB Touche2020
      config: default
      split: test
      revision: 527b7d77e16e343303e68cb6af11d6e18b9f7b3b
    metrics:
    - type: map_at_1
      value: 1.49
    - type: map_at_10
      value: 6.39
    - type: map_at_100
      value: 11.424
    - type: map_at_1000
      value: 12.847
    - type: map_at_3
      value: 3.055
    - type: map_at_5
      value: 3.966
    - type: ndcg_at_1
      value: 17.347
    - type: ndcg_at_10
      value: 16.904
    - type: ndcg_at_100
      value: 29.187
    - type: ndcg_at_1000
      value: 40.994
    - type: ndcg_at_3
      value: 15.669
    - type: ndcg_at_5
      value: 16.034000000000002
    - type: precision_at_1
      value: 18.367
    - type: precision_at_10
      value: 16.326999999999998
    - type: precision_at_100
      value: 6.673
    - type: precision_at_1000
      value: 1.439
    - type: precision_at_3
      value: 17.687
    - type: precision_at_5
      value: 17.143
    - type: recall_at_1
      value: 1.49
    - type: recall_at_10
      value: 12.499
    - type: recall_at_100
      value: 41.711
    - type: recall_at_1000
      value: 78.286
    - type: recall_at_3
      value: 4.055000000000001
    - type: recall_at_5
      value: 6.5040000000000004
  - task:
      type: Classification
    dataset:
      type: mteb/toxic_conversations_50k
      name: MTEB ToxicConversationsClassification
      config: default
      split: test
      revision: edfaf9da55d3dd50d43143d90c1ac476895ae6de
    metrics:
    - type: accuracy
      value: 66.9918
    - type: ap
      value: 12.24755801720171
    - type: f1
      value: 51.31653313211933
  - task:
      type: Classification
    dataset:
      type: mteb/tweet_sentiment_extraction
      name: MTEB TweetSentimentExtractionClassification
      config: default
      split: test
      revision: 62146448f05be9e52a36b8ee9936447ea787eede
    metrics:
    - type: accuracy
      value: 55.410299943406905
    - type: f1
      value: 55.71547395803944
  - task:
      type: Clustering
    dataset:
      type: mteb/twentynewsgroups-clustering
      name: MTEB TwentyNewsgroupsClustering
      config: default
      split: test
      revision: 091a54f9a36281ce7d6590ec8c75dd485e7e01d4
    metrics:
    - type: v_measure
      value: 46.860271427647774
  - task:
      type: PairClassification
    dataset:
      type: mteb/twittersemeval2015-pairclassification
      name: MTEB TwitterSemEval2015
      config: default
      split: test
      revision: 70970daeab8776df92f5ea462b6173c0b46fd2d1
    metrics:
    - type: cos_sim_accuracy
      value: 84.1151576563152
    - type: cos_sim_ap
      value: 67.85802440228593
    - type: cos_sim_f1
      value: 64.08006919560113
    - type: cos_sim_precision
      value: 60.260283523123405
    - type: cos_sim_recall
      value: 68.41688654353561
    - type: dot_accuracy
      value: 84.1151576563152
    - type: dot_ap
      value: 67.85802503410727
    - type: dot_f1
      value: 64.08006919560113
    - type: dot_precision
      value: 60.260283523123405
    - type: dot_recall
      value: 68.41688654353561
    - type: euclidean_accuracy
      value: 84.1151576563152
    - type: euclidean_ap
      value: 67.85802845168082
    - type: euclidean_f1
      value: 64.08006919560113
    - type: euclidean_precision
      value: 60.260283523123405
    - type: euclidean_recall
      value: 68.41688654353561
    - type: manhattan_accuracy
      value: 83.96614412588663
    - type: manhattan_ap
      value: 67.66935451307549
    - type: manhattan_f1
      value: 63.82363570654138
    - type: manhattan_precision
      value: 58.72312125914432
    - type: manhattan_recall
      value: 69.89445910290237
    - type: max_accuracy
      value: 84.1151576563152
    - type: max_ap
      value: 67.85802845168082
    - type: max_f1
      value: 64.08006919560113
  - task:
      type: PairClassification
    dataset:
      type: mteb/twitterurlcorpus-pairclassification
      name: MTEB TwitterURLCorpus
      config: default
      split: test
      revision: 8b6510b0b1fa4e4c4f879467980e9be563ec1cdf
    metrics:
    - type: cos_sim_accuracy
      value: 88.2504754142896
    - type: cos_sim_ap
      value: 84.70165951451109
    - type: cos_sim_f1
      value: 76.57057281916886
    - type: cos_sim_precision
      value: 74.5226643346451
    - type: cos_sim_recall
      value: 78.73421619956883
    - type: dot_accuracy
      value: 88.2504754142896
    - type: dot_ap
      value: 84.7016596919848
    - type: dot_f1
      value: 76.57057281916886
    - type: dot_precision
      value: 74.5226643346451
    - type: dot_recall
      value: 78.73421619956883
    - type: euclidean_accuracy
      value: 88.2504754142896
    - type: euclidean_ap
      value: 84.70166029488888
    - type: euclidean_f1
      value: 76.57057281916886
    - type: euclidean_precision
      value: 74.5226643346451
    - type: euclidean_recall
      value: 78.73421619956883
    - type: manhattan_accuracy
      value: 88.27376101214732
    - type: manhattan_ap
      value: 84.63518812822186
    - type: manhattan_f1
      value: 76.55138674594514
    - type: manhattan_precision
      value: 74.86934118513065
    - type: manhattan_recall
      value: 78.31074838312288
    - type: max_accuracy
      value: 88.27376101214732
    - type: max_ap
      value: 84.70166029488888
    - type: max_f1
      value: 76.57057281916886
---

# all-MiniLM-L6-v2
This is a [sentence-transformers](https://www.SBERT.net) model: It maps sentences & paragraphs to a 384 dimensional dense vector space and can be used for tasks like clustering or semantic search.

## Usage (Sentence-Transformers)
Using this model becomes easy when you have [sentence-transformers](https://www.SBERT.net) installed:

```
pip install -U sentence-transformers
```

Then you can use the model like this:
```python
from sentence_transformers import SentenceTransformer
sentences = ["This is an example sentence", "Each sentence is converted"]

model = SentenceTransformer('sentence-transformers/all-MiniLM-L6-v2')
embeddings = model.encode(sentences)
print(embeddings)
```

## Usage (HuggingFace Transformers)
Without [sentence-transformers](https://www.SBERT.net), you can use the model like this: First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.

```python
from transformers import AutoTokenizer, AutoModel
import torch
import torch.nn.functional as F

#Mean Pooling - Take attention mask into account for correct averaging
def mean_pooling(model_output, attention_mask):
    token_embeddings = model_output[0] #First element of model_output contains all token embeddings
    input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
    return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)


# Sentences we want sentence embeddings for
sentences = ['This is an example sentence', 'Each sentence is converted']

# Load model from HuggingFace Hub
tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')
model = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L6-v2')

# Tokenize sentences
encoded_input = tokenizer(sentences, padding=True, truncation=True, return_tensors='pt')

# Compute token embeddings
with torch.no_grad():
    model_output = model(**encoded_input)

# Perform pooling
sentence_embeddings = mean_pooling(model_output, encoded_input['attention_mask'])

# Normalize embeddings
sentence_embeddings = F.normalize(sentence_embeddings, p=2, dim=1)

print("Sentence embeddings:")
print(sentence_embeddings)
```

## Evaluation Results

For an automated evaluation of this model, see *MTEB*: https://huggingface.co/spaces/mteb/leaderboard or the *Sentence Embeddings Benchmark*: [https://seb.sbert.net](https://seb.sbert.net?model_name=sentence-transformers/all-MiniLM-L12-v2)

------

## Background

The project aims to train sentence embedding models on very large sentence level datasets using a self-supervised 
contrastive learning objective. We used the pretrained [`nreimers/MiniLM-L6-H384-uncased`](https://huggingface.co/nreimers/MiniLM-L6-H384-uncased) model and fine-tuned in on a 
1B sentence pairs dataset. We use a contrastive learning objective: given a sentence from the pair, the model should predict which out of a set of randomly sampled other sentences, was actually paired with it in our dataset.

We developped this model during the 
[Community week using JAX/Flax for NLP & CV](https://discuss.huggingface.co/t/open-to-the-community-community-week-using-jax-flax-for-nlp-cv/7104), 
organized by Hugging Face. We developped this model as part of the project:
[Train the Best Sentence Embedding Model Ever with 1B Training Pairs](https://discuss.huggingface.co/t/train-the-best-sentence-embedding-model-ever-with-1b-training-pairs/7354). We benefited from efficient hardware infrastructure to run the project: 7 TPUs v3-8, as well as intervention from Googles Flax, JAX, and Cloud team member about efficient deep learning frameworks.

## Intended uses

Our model is intented to be used as a sentence and short paragraph encoder. Given an input text, it ouptuts a vector which captures 
the semantic information. The sentence vector may be used for information retrieval, clustering or sentence similarity tasks.

By default, input text longer than 256 word pieces is truncated.


## Training procedure

### Pre-training 

We use the pretrained [`nreimers/MiniLM-L6-H384-uncased`](https://huggingface.co/nreimers/MiniLM-L6-H384-uncased) model. Please refer to the model card for more detailed information about the pre-training procedure.

### Fine-tuning 

We fine-tune the model using a contrastive objective. Formally, we compute the cosine similarity from each possible sentence pairs from the batch.
We then apply the cross entropy loss by comparing with true pairs.

#### Hyper parameters

We trained ou model on a TPU v3-8. We train the model during 100k steps using a batch size of 1024 (128 per TPU core).
We use a learning rate warm up of 500. The sequence length was limited to 128 tokens. We used the AdamW optimizer with
a 2e-5 learning rate. The full training script is accessible in this current repository: `train_script.py`.

#### Training data

We use the concatenation from multiple datasets to fine-tune our model. The total number of sentence pairs is above 1 billion sentences.
We sampled each dataset given a weighted probability which configuration is detailed in the `data_config.json` file.


| Dataset                                                  | Paper                                    | Number of training tuples  |
|--------------------------------------------------------|:----------------------------------------:|:--------------------------:|
| [Reddit comments (2015-2018)](https://github.com/PolyAI-LDN/conversational-datasets/tree/master/reddit) | [paper](https://arxiv.org/abs/1904.06472) | 726,484,430 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Abstracts) | [paper](https://aclanthology.org/2020.acl-main.447/) | 116,288,806 |
| [WikiAnswers](https://github.com/afader/oqa#wikianswers-corpus) Duplicate question pairs | [paper](https://doi.org/10.1145/2623330.2623677) | 77,427,422 |
| [PAQ](https://github.com/facebookresearch/PAQ) (Question, Answer) pairs | [paper](https://arxiv.org/abs/2102.07033) | 64,371,441 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Titles) | [paper](https://aclanthology.org/2020.acl-main.447/) | 52,603,982 |
| [S2ORC](https://github.com/allenai/s2orc) (Title, Abstract) | [paper](https://aclanthology.org/2020.acl-main.447/) | 41,769,185 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Body) pairs  | - | 25,316,456 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title+Body, Answer) pairs  | - | 21,396,559 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Answer) pairs  | - | 21,396,559 |
| [MS MARCO](https://microsoft.github.io/msmarco/) triplets | [paper](https://doi.org/10.1145/3404835.3462804) | 9,144,553 |
| [GOOAQ: Open Question Answering with Diverse Answer Types](https://github.com/allenai/gooaq) | [paper](https://arxiv.org/pdf/2104.08727.pdf) | 3,012,496 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 1,198,260 |
| [Code Search](https://huggingface.co/datasets/code_search_net) | - | 1,151,414 |
| [COCO](https://cocodataset.org/#home) Image captions | [paper](https://link.springer.com/chapter/10.1007%2F978-3-319-10602-1_48) | 828,395|
| [SPECTER](https://github.com/allenai/specter) citation triplets | [paper](https://doi.org/10.18653/v1/2020.acl-main.207) | 684,100 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Question, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 681,164 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Question) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 659,896 |
| [SearchQA](https://huggingface.co/datasets/search_qa) | [paper](https://arxiv.org/abs/1704.05179) | 582,261 |
| [Eli5](https://huggingface.co/datasets/eli5) | [paper](https://doi.org/10.18653/v1/p19-1346) | 325,475 |
| [Flickr 30k](https://shannon.cs.illinois.edu/DenotationGraph/) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/229/33) | 317,695 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles) | | 304,525 |
| AllNLI ([SNLI](https://nlp.stanford.edu/projects/snli/) and [MultiNLI](https://cims.nyu.edu/~sbowman/multinli/) | [paper SNLI](https://doi.org/10.18653/v1/d15-1075), [paper MultiNLI](https://doi.org/10.18653/v1/n18-1101) | 277,230 | 
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (bodies) | | 250,519 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles+bodies) | | 250,460 |
| [Sentence Compression](https://github.com/google-research-datasets/sentence-compression) | [paper](https://www.aclweb.org/anthology/D13-1155/) | 180,000 |
| [Wikihow](https://github.com/pvl/wikihow_pairs_dataset) | [paper](https://arxiv.org/abs/1810.09305) | 128,542 |
| [Altlex](https://github.com/chridey/altlex/) | [paper](https://aclanthology.org/P16-1135.pdf) | 112,696 |
| [Quora Question Triplets](https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs) | - | 103,663 |
| [Simple Wikipedia](https://cs.pomona.edu/~dkauchak/simplification/) | [paper](https://www.aclweb.org/anthology/P11-2117/) | 102,225 |
| [Natural Questions (NQ)](https://ai.google.com/research/NaturalQuestions) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/1455) | 100,231 |
| [SQuAD2.0](https://rajpurkar.github.io/SQuAD-explorer/) | [paper](https://aclanthology.org/P18-2124.pdf) | 87,599 |
| [TriviaQA](https://huggingface.co/datasets/trivia_qa) | - | 73,346 |
| **Total** | | **1,170,060,424** |
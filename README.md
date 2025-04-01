# Table. Hyperparameters used in the experiment.

| Hyperparameter            | Antmaze                   | Adroit                    | RLBench                   |
|---------------------------|---------------------------|---------------------------|---------------------------|
| **PORL**                  |                           |                           |                           |
| Epsilon                   | 0.1                       | 0.1                       | 0.1                       |
| Pre-sample steps          | 20k                       | 5k                        | 20k                       |
| **Optimization**          |                           |                           |                           |
| Actor Learning Rate       | 1𝑒 − 4                    | 1𝑒 − 4                    | 1𝑒 − 4                    |
| Critic Learning Rate      | 3𝑒 − 4                    | 3𝑒 − 4                    | 3𝑒 − 4                    |
| Temperature Learning Rate | 1𝑒 − 4                    | 1𝑒 − 4                    | 1𝑒 − 4                    |
| Batch Size                | 512                       | 512                       | 512                       |
| Optimizer                 | Adam                      | Adam                      | Adam                      |
| UTD                       | 16                        | 16                        | 16                        |
| Offline Steps             | 1000,000                  | 40,000                    | -                         |
| **Architecture**          |                           |                           |                           |
| Actor Network             | [256, 256]                | [512, 512]                | [256, 256]                |
| Critic Network            | [256, 256, 256, 256]      | [512, 512, 512]           | [256, 256, 256, 256]      |
| Q-ensemble                | 10                        | 10                        | 10                        |
| Activations               | Relu                      | Relu                      | Relu                      |


# Table. Asymptotic performance in the Antmaze experiments.

| Task                     | AWAC       | CQL        | Cal-QL     | IQL        | JSRL       | RLPD       | WSRL       | PORL       |
|--------------------------|------------|------------|------------|------------|------------|------------|------------|------------|
| antmaze-large-diverse    | 0.00±0.00  | 70.39±4.54 | 87.69±3.49 | 53.97±4.05 | 0.00±0.00  | 81.13±3.59 | 97.00±1.62 | 97.50±1.52 |
| antmaze-large-play       | 0.00±0.00  | 77.83±4.21 | 85.69±3.13 | 57.09±3.36 | 0.00±0.00  | 75.84±2.72 | 88.67±9.03 | 97.67±1.17 |
| antmaze-medium-diverse   | 0.12±0.11  | 90.17±1.71 | 97.21±1.30 | 89.55±2.24 | 98.33±1.83 | 95.97±1.39 | 98.78±0.50 | 99.42±0.49 |
| antmaze-medium-play      | 0.00±0.00  | 93.89±2.07 | 96.88±1.38 | 87.76±2.14 | 98.33±1.05 | 96.32±1.30 | 99.44±0.78 | 98.33±0.92 |
| antmaze-umaze            | 95.00±3.04 | 98.75±0.52 | 99.50±0.42 | 92.79±2.31 | 99.72±0.68 | 96.83±0.93 | 99.78±0.34 | 99.78±0.34 |
| antmaze-umaze-diverse    | 0.00±0.00  | 89.00±2.96 | 94.93±2.26 | 34.76±3.84 | 99.44±0.86 | 97.62±1.18 | 100.00±0.00 | 99.44±0.27 |
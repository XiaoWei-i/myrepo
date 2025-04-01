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
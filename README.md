# FastGen
This repo contains the source code for: Model Tells You What to Discard: Adaptive KV Cache Compression for LLMs

For now, please check the community reproduction here: https://github.com/AnswerDotAI/cold-compress/tree/main
The repo is develope by answer.ai and contains a reproduction of FastGen algorithm, and a wide range of other compression strategies.

Meanwhile, Microsoft Research Asia releases MInference https://github.com/microsoft/MInference/tree/main, which is a close implementation of the FastGen algorithm. The core part of the algorithm, for each attention head and each data instance, at the end of prefilling stage, profile the attention matrix, and pick a hybrid portfolio of eviction strategies(special tokens, local, topk...) based on the profiling.

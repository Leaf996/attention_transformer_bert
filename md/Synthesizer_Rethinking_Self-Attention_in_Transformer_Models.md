# Rethinking Self-Attention in Transformer Models
## Questions
- TODO
## Abstract
- The dot product self-attention is known to be **central and indispensable** to state-of-the-art Transformer models.
- Via extensive experiments, we find that:
    - random alignment matrices surprisingly perform quite competitively
    - learning attention weights from token-token(query-key) interactions is not that important after all
## Introduction
- Transformer models have demonstrated success across a wide range of tasks.
- Indeed, the term `query, keys, and values` imply that self-attention emulates a content-based retrieval process which leverages pairwise interactions at its very core.
- Moving against convention, this paper postulates that `we can not only do without dot product self-attention but also content-based memory-like self-attention algotether`.
- Aside from generalizing the standard Transformer model, we show that it is possible to achieve competitive results with fully golbal attention weights that do not consider token-token interactions or any instance-level(local) information at all.
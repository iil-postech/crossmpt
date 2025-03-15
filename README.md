# CrossMPT: Cross-attention message-passing transformer for error correcting codes

This repository is the official implementation of the ICLR 2025 "CrossMPT: Cross-attention message-passing transformer for error correcting codes"

# [Paper]([https://arxiv.org/abs/2308.08128](https://openreview.net/forum?id=gFvRRCnQvX))
<p align="center"><img src="https://github.com/user-attachments/assets/9623e0e2-eebd-4479-a28f-fc1308d76c65" width="900"/>

# Experimental Results
<p align="center"><img src="https://github.com/user-attachments/assets/a658c814-cb91-4a2d-a581-b4e6f02ad2ea" width="900"/>

BER performance of various decoders (BP, Hyp BP, AR BP, ECCT) and CrossMPT for $$N=6$$ and $$d=128$$ (left). Performance comparison between BP decoder (iteration 20, 50, and 100) and CrossMPT for $$N=10$$ and $$d=128$$ (right).


# Installation
* Pytorch

# Running the code

Codes for training CrossMPT on GPU 0, 6 decoder layers, dimension 128 on LDPC codes (121,60)

```python
python Main.py --gpu=0 --N_dec=6 --d_model=128 --code_type=LDPC --code_n=121--code_k=60
```

# Code arguments
```
--epochs                   number of epoch
--batch_size               batch size
--code_type                code type, 'BCH' or 'POLAR'
--code_k                   codeword dimension k
--code_n                   codeword length n
--N_dec                    number of decoder layers N
--d_model                  embedding vector dimension d
```

# Citation

```
@inproceedings{
park2025crossmpt,
title={Cross{MPT}: Cross-attention Message-passing Transformer for Error Correcting Codes},
author={Seong-Joon Park and Hee-Youl Kwak and Sang-Hyo Kim and Yongjune Kim and Jong-Seon No},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://openreview.net/forum?id=gFvRRCnQvX}
}
```

# License

Codes are available only for non-commercial research purposes.

# Acknowledgement

This repository is based on [***ECCT***](https://github.com/yoniLc/ECCT).

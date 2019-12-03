# 2PCNN

Demonstration code for two-particle correlation neural network (2PCNN). 
See the reference for more information:
https://arxiv.org/abs/1911.02020

## File descriptions:
* prototype_train.py
> a code to construct a 2PCNN prototype model with only energy flow information (pt, eta, phi for 2 particles), 
> loading the jet data, and training with early stopping enabled.
> Recommened to increase the data statistics for a serious training.
* prototype_deploy.py
> similar to the previous code, instead of training, only construct the same model, loading the trained weights,
> and produce the resulting scores and ROC curve.
* wgts_2pcnn_fatjet_w_vs_q.h5
* wgts_2pcnn_fatjet_t_vs_q.h5
> pre-trained weights for W-jet versus quark-jet (2-prong versus 1-prong), and 
> for top-jet versus quark-jet (3-prong versus 1-prong). 

## Test samples:
https://drive.google.com/drive/u/0/folders/1HojGLS_ODr7E7tndy2vz0fxRB2N10VAR
* fatjet_t_match_vz_to_tt.txt.gz
* fatjet_w_match_vz_to_ww.txt.gz
* fatjet_q_match_vz_to_qq.txt.gz
> The files are simple gziped text file (no needs of unzip). See the parse_jet_data() function in the demo code 
> for exact data format.

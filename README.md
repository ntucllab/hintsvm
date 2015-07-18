hintsvm
===================

hintsvm implements the active learning algorithm described in "Active Learning with
Hinted Support Vector Machine." by Li, Chun-Liang, Chun-Sung Ferng, and Hsuan-Tien Lin.

hintsvm is based on libsvm, modified from libsvm3.1.

There are two parameters added to the original libsvm:

1. '-s 5' for hintsvm.
2. '-W weight file'.

Usage:
	Use '-W weight_file' to assign weights for each instance which is used
    to adjust the weight of labeled and unlabeled instances.
	Please make sure all weights are non-negative.

Example:
	./svm-train -W heart_scale.wgt  heart_scale

For now only the python wrapper are supported.

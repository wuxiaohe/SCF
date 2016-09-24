____________________________________________________
Project webpage: http://arxiv.org/pdf/1601.06032.pdf

This MATLAB code implements a simple tracking pipeline based on the SCF, MSCF, KSCF and SKSCF.

Detailed Information:
1. The MSCF.zip implements the SCF and MSCF by setting 'feature_type' variable to 'gray' and 'HOG_CN_Color' respectively.
2. The KSCF.zip implements the kernel SCF.
3. The SKSCF.zip implements the scale-adaptive kernel SCF.

For SCF, MSCF, KSCF and SKSCF, we provide the simplified version code with updating the filter only once. 
The optimal iterations should be 5~10 in 'MSCF.m', 'KSCF.m' and 'SKSCF.m'.
__________
Quickstart

1. Extract code somewhere.

2. The tracker is available for the 50 videos of the Visual Tracking
   Benchmark [3]. You need to put all videos under the default location 'base_path' in 'run.m'.

3. The videos can be downloaded from http://cvlab.hanyang.ac.kr/tracker_benchmark/datasets.html.

4. Execute 'run' without parameters to test on it. For SCF, do not forget to change the 'feature_type' variable to 'gray'.


Note: The tracker uses the 'fhog'/'gradientMex' functions from Piotr's Toolbox.
Some pre-compiled MEX files are provided for convenience. If they do not work for your
system, just get the toolbox from http://vision.ucsd.edu/~pdollar/toolbox/doc/index.html

__________
References

[1] J. F. Henriques, R. Caseiro, P. Martins, J. Batista, "High-Speed Tracking with
Kernelized Correlation Filters", TPAMI 2014.

[2] J. F. Henriques, R. Caseiro, P. Martins, J. Batista, "Exploiting the Circulant
Structure of Tracking-by-detection with Kernels", ECCV 2012.

[3] Y. Wu, J. Lim, M.-H. Yang, "Online Object Tracking: A Benchmark", CVPR 2013.
Website: http://visual-tracking.net/

________
Citation

If you find the code and dataset useful in your research, please consider citing:

@article{zuo2016learning,
  title={Learning Support Correlation Filters for Visual Tracking},
  author={Zuo, Wangmeng and Wu, Xiaohe and Lin, Liang and Zhang, Lei and Yang, Ming-Hsuan},
  journal={arXiv preprint arXiv:1601.06032},
  year={2016}
}

________
Contents

|  Folder    | description |
| ---|---|

Feedbacks and comments are welcome! Feel free to contact us via [lotuswxh@gmail.com] or [angela612@126.com].

________
Liscense
Copyright (c) 2016, Xiaohe Wu
All rights reserved. 
Redistribution and use in source and binary forms, with or without modification, are 
permitted provided that the following conditions are met:
* Redistributions of source code must retain the above copyright 
  notice, this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright 
  notice, this list of conditions and the following disclaimer in 
  the documentation and/or other materials provided with the distribution
        
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" 
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE 
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE 
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE 	
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR 
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF 
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS 
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
POSSIBILITY OF SUCH DAMAGE.

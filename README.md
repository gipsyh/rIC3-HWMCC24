# rIC3-HWMCC24
rIC3 model checker for Hardware Model Checking Competition 2024([HWMCC'24](https://hwmcc.github.io/2024)) submission.

Our experiments show that it can solve 299 out of the total 324 cases in the bv track of [HWMCC'20](https://fmv.jku.at/hwmcc20/hwmcc20slides.pdf), which is 37 more cases than the most solved checker, abc-superprove, in HWMCC'20.

# Usage
The default configuration is the portfolio of 16 threads by using the IC3, BMC and K-induction algorithms.

For models in aiger format:
```
rIC3 <aiger model path> [certification path]
```
If the certification path is not specified, rIC3 will not output the certification in [certifaiger](https://github.com/Froleyks/certifaiger) format or the counter-example in [aiger](https://github.com/arminbiere/aiger) witness format.

For models in btor2 format:
```
rIC3 <btor2 model path>
```
For btor model, the model file name should be suffixed with **.btor** or **.btor2**, otherwise, it will be recognized as an aiger model. rIC3 does not support outputting certification or the counter-example of btor2 models.

# Authers
Yuheng Su, gipsyh.icu@gmail.com

University of Chinese Academy of Sciences; Institute of Software, Chinese Academy of Sciences
 
Qiusong Yang, qiusong@iscas.ac.cn

Institute of Software, Chinese Academy of Sciences

Yiwei Ci, yiwei@iscas.ac.cn

Institute of Software, Chinese Academy of Sciences

# rIC3-HWMCC24
rIC3 model checker for Hardware Model Checking Competition 2024(HWMCC'24) submission.

rIC3 is competitive, as my experiments show that it can solve 299 out of the total 324 cases in the bv track of HWMCC'20, which is 37 more cases solved than the most solved checker abc-superprove in HWMCC'20.

# Usage
For models in aiger format:
```
rIC3 <aiger model path> [certifaiger path]
```
If the certifier path is not specified, rIC3 will not output the witness circuit or the counter-example.

For models in btor2 format:
```
rIC3 <btor2 model path>
```
For now, rIC3 does not support outputting certification or the counter-example of btor2 models.
# Authers
Yuheng Su, gipsyh.icu@gmail.com

University of Chinese Academy of Sciences

Institute of Software, Chinese Academy of Sciences
 
Qiusong Yang, qiusong@iscas.ac.cn

Institute of Software, Chinese Academy of Sciences

Yiwei Ci, yiwei@iscas.ac.cn

Institute of Software, Chinese Academy of Sciences

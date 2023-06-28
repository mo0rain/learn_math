

常见DSA参数（p、q、签名）长度为：
- 1024  160       320
- 2048  224       448
- 3072  256       512
下面以1024位的DSA为例进行说明：

## 密钥生成
1.生成一个素数p，且$\Huge 2^{1023}<p<2^{1024}$
2.找到p-1的一个素除数q，且$\Huge 2^{159}<q<2^{160}$
3.找到ord(α)=q的元素α，即α生成了拥有q个元素的子群
4.选择一个随机整数d，且0 < d < q
5.计算 β 三 $\Huge α^d$ mod p
密钥为
公钥: (p,q,α,β)
私钥: (d)


## 签名生成



## 签名验证



## 正确性验证




# Reference

[DSA签名算法简介\_alwaysrun的博客-CSDN博客](https://blog.csdn.net/alwaysrun/article/details/89076605 "DSA签名算法简介\_alwaysrun的博客-CSDN博客")


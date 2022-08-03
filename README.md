# xunfei2022BrainVesselSegementation
使用monai+pytorch-lightning版本最高得分为0.84左右。  
使用nnunet版本最高得分为0.89左右，最终初榜排名为15。  
nnunet版本中使用了fsl工具包里面的bet2算法去除颅骨和头皮。  
注意事项：  
 1、后续者可试试将nnunet版本的优化器从sgd更换为adamw，学习率控制使用余弦退火，不过这需要手动安装nnunet版本改起来方便点，本人通过pip命令安装的nnunet，所以就没有试过这个思路。  
 2、monai版本运行时直接运行main.py,在该版本中我试过了随机翻转，随机旋转，随机缩放，高斯噪声等（基本把nnunet的数据增强方法都试过一遍），但是效果均不如不使用任何数据增强训练出来的模型，我不知道是不是自己哪里没写对，如果后续者发现了我的问题，欢迎和我联系探讨，QQ：1152545264

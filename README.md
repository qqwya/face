# face
1.FReeNet: Multi-Identity Face Reenactment

作者 | Jiangning Zhang, Xianfang Zeng, Mengmeng Wang, Yusu Pan, Liang Liu, Yong Liu, Yu Ding, Changjie Fan
代码 | https://github.com/zhangzjn/FReeNet
论文 | https://arxiv.org/abs/1905.11805
单位 | 浙大，网易伏羲AI Lab
完成的是面部重演工作（生成的图像保留参考图像的身份以及源图像的表情），作者团队来自浙大和网易。
https://github.com/qqwya/face/blob/main/image/FREEnet.jpg

2.Cascade EF-GAN: Progressive Facial Expression Editing With Local Focuses

作者 | Rongliang Wu, Gongjie Zhang, Shijian Lu, Tao Chen
论文 | https://arxiv.org/abs/2003.05905
单位 | 南洋理工大学，复旦大学
将给定面部图像的表情转换为目标表情，而不会丢失身份属性
在人脸编辑里，当前的方法仍然可能产生伪影和模糊（例如在处理诸如从愤怒到笑之类的大幅表情转换时）。
为了解决这些局限性，提出Cascade Expression Focal GAN（Cascade EF-GAN）能够以局部表情为重点进行渐进式表情编辑。通过将大幅度表情转换分成多个小面部表情来设计级联式的转换，有助于抑制重叠的伪像并产生更逼真自然的效果。

3.MaskGAN: Towards Diverse and Interactive Facial Image Manipulation

作者 | Cheng-Han Lee, Ziwei Liu, Lingyun Wu, Ping Luo
代码 | https://github.com/switchablenorms/CelebAMask-HQ
论文 | https://arxiv.org/abs/2002.11841
单位 | 商汤科技；香港中文大学；香港大学
尽管人脸图像处理已取得了巨大发展，但大多数方法要么在一组预定义的面部属性上进行操作，要么只能给用户提供很小的交互操作自由空间。本文提出为MaskGAN，可进行多种交互式的人脸编辑。
本文关键之处是，语义mask可作为具有高保真度、灵活的面部操作的中间表示。MaskGAN具有两个主要组件：1）密集映射网络（DMN）和 2）编辑行为模拟训练（EBST）。具体来说，DMN学习用户自由修改的mask和目标图像之间的映射，实现多种生成结果。 EBST在源mask上对用户编辑行为进行建模，从而使整个框架对各种操纵的输入更加健壮。具体来说，它引入了dual-editing consistency作为辅助监督。
为便于进行广泛的研究，还构建了一个名为CelebAMask-HQ的细粒度mask的、大规模高分辨率数据集。
这个工作的主要idea是用一个叫做DMN的网络，把人脸mask和人脸对应起来，也就是可以很好地从人脸mask映射到真实人脸图像。然后对人脸mask进行编辑，在通过DMN就得到与之对应的编辑人脸。

4.Interpreting the Latent Space of GANs for Semantic Face Editing

作者 | Yujun Shen, Jinjin Gu, Xiaoou Tang, Bolei Zhou
代码 | https://github.com/genforce/interfacegan
论文 | https://arxiv.org/abs/1907.10786
单位 | 香港中文大学，香港中文大学（深圳）
对GAN如何将从随机分布中采样的潜码映射到真实图像仍缺乏足够的了解。
在这项工作中，提出了一个称为InterFaceGAN的新颖框架，用于通过解释GAN所学到的潜在语义来进行人脸编辑。
作者发现，训练好的生成模型的潜码实际上在线性变换后即可学到解纠缠的表示。作者探索了各种语义之间的纠缠现象，并尝试对人脸属性进行更精确控制生成。
5.CONFIG: Controllable Neural Face Image Generation

作者 | Marek Kowalski, Stephan J. Garbin, Virginia Estellers, Tadas Baltrušaitis, Matthew Johnson, Jamie Shotton
单位 | 微软
论文 | https://arxiv.org/abs/2005.02671
代码 | https://github.com/microsoft/ConfigNet

6.CAFE-GAN: Arbitrary Face Attribute Editing with Complementary Attention Feature

作者 | Jeong gi Kwak, David K. Han, Hanseok Ko
单位 | 高丽大学；ARL
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123590511.pdf
人脸属性编辑

7.CooGAN: A Memory-Efficient Framework for High-Resolution Facial Attribute Editing

作者 | Xuanhong Chen, Bingbing Ni, Naiyuan Liu, Ziang Liu, Yiliu Jiang, Loc Truong, Qi Tian
单位 | 上海交通大学；Huawei HiSilicon；华为
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560647.pdf
代码 | https://github.com/XHChen0528/CooGAN
人脸属性编辑

8.SSCGAN: Facial Attribute Editing via Style Skip Connections
作者 | Wenqing Chu, Ying Tai, Chengjie Wang, Jilin Li, Feiyue Huang, Rongrong Ji
单位 | 腾讯优图；厦门大学
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123600409.pdf

9.Toward Fine-grained Facial Expression Manipulation

作者 | Jun Ling, Han Xue, Li Song, Shuhui Yang, Rong Xie, Xiao Gu
单位 | 上海交通大学
论文 | https://arxiv.org/abs/2004.03132
代码 | https://github.com/junleen/Expression-manipulato


10.Learning Formation of Physically-Based Face Attributes
作者 | Ruilong Li, Karl Bladin, Yajie Zhao, Chinmay Chinara, Owen Ingraham, Pengda Xiang, Xinglei Ren, Pratusha Prasad, Bipin Kishore, Jun Xing, Hao Li
单位 | USC Institute for Creative Technologies，南加州大学，Pinscreen
论文 | https://arxiv.org/abs/2004.03458
进行id和表情的解缠，提供低维特征向量控制面部

11.FaceScape: A Large-Scale High Quality 3D Face Dataset and Detailed Riggable 3D Face Prediction

作者 | Haotian Yang, Hao Zhu, Yanru Wang, Mingkai Huang, Qiu Shen, Ruigang Yang, Xun Cao
代码 | https://github.com/zhuhao-nju/facescape
该论文发布大尺度高精度人脸三维模型数据库FaceScape，并首次提出从单幅图像预测高精度、可操控人脸三维模型的方法。FaceScape数据库包含约18000个高精度三维面部模型，每个模型包含基底模型和4K分辨率的置换图及纹理贴图，能够表征出面部极细微的三维结构和纹理。与现有公开的三维人脸数据库相比，FaceScape在模型数量和质量上均处于世界最高水准。
在FaceScape数据库的基础之上，本文还探索了一项具有挑战性的新课题：以单幅人脸图像为输入，预测高精度、表情可操控的三维人脸模型。该方法的预测结果能够通过表情操控生成精细的面部模型序列，所生成的模型在新表情下仍然包含逼真的细节三维结构。据悉，FaceScape数据库和代码将于近期免费发布，供非商业用途的学术研究使用。

12.Adversarial Latent Autoencoders
作者 | Stanislav Pidhorskyi, Donald Adjeroh, Gianfranco Doretto
论文 | https://arxiv.org/abs/2004.03132
代码 | https://github.com/podgorskiy/ALAE
本文提出的Adversarial Latent Autoencoder (ALAE)是一种结合了自编码器、更具通用性的、利用GAN方法的架构，它可以进行更“解耦”的表征学习。
ALAE不仅可以生成可以和StyleGAN媲美的1024大图，还可以对真实image进行更好的重建、编辑等。

13.StyleRig: Rigging StyleGAN for 3D Control over Portrait Images
论文 | https://arxiv.org/pdf/2004.00121.pdf
StyleGAN可以生成具有极具真实感的肖像图像，但缺乏对3D可解释的语义参数（如脸部姿势，表情，和场景照明）。
3DMM提供了语义参数以控制，但是在渲染时缺乏真实感，且仅对人脸进行建模，而对肖像其他部分（头发、嘴部内部、背景）不进行建模。
本文提出通过3DMM对预训练、固定的StyleGAN进行面部语义参数控制的方法；方法以自监督式训练，无需人工标注


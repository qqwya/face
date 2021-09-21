# face
1.FReeNet: Multi-Identity Face Reenactment

作者 | Jiangning Zhang, Xianfang Zeng, Mengmeng Wang, Yusu Pan, Liang Liu, Yong Liu, Yu Ding, Changjie Fan
代码 | https://github.com/zhangzjn/FReeNet
论文 | https://arxiv.org/abs/1905.11805
单位 | 浙大，网易伏羲AI Lab
完成的是面部重演工作（生成的图像保留参考图像的身份以及源图像的表情），作者团队来自浙大和网易。
![image](https://user-images.githubusercontent.com/36876387/134147325-43bb1b50-4087-4aa1-b7dd-4973b106be1b.png)

2.Cascade EF-GAN: Progressive Facial Expression Editing With Local Focuses

作者 | Rongliang Wu, Gongjie Zhang, Shijian Lu, Tao Chen
论文 | https://arxiv.org/abs/2003.05905
单位 | 南洋理工大学，复旦大学
将给定面部图像的表情转换为目标表情，而不会丢失身份属性
在人脸编辑里，当前的方法仍然可能产生伪影和模糊（例如在处理诸如从愤怒到笑之类的大幅表情转换时）。
为了解决这些局限性，提出Cascade Expression Focal GAN（Cascade EF-GAN）能够以局部表情为重点进行渐进式表情编辑。通过将大幅度表情转换分成多个小面部表情来设计级联式的转换，有助于抑制重叠的伪像并产生更逼真自然的效果。
![image](https://user-images.githubusercontent.com/36876387/134147398-055a9553-0656-43ea-84dd-a818088ab529.png)

3.MaskGAN: Towards Diverse and Interactive Facial Image Manipulation

作者 | Cheng-Han Lee, Ziwei Liu, Lingyun Wu, Ping Luo
代码 | https://github.com/switchablenorms/CelebAMask-HQ
论文 | https://arxiv.org/abs/2002.11841
单位 | 商汤科技；香港中文大学；香港大学
尽管人脸图像处理已取得了巨大发展，但大多数方法要么在一组预定义的面部属性上进行操作，要么只能给用户提供很小的交互操作自由空间。本文提出为MaskGAN，可进行多种交互式的人脸编辑。
本文关键之处是，语义mask可作为具有高保真度、灵活的面部操作的中间表示。MaskGAN具有两个主要组件：1）密集映射网络（DMN）和 2）编辑行为模拟训练（EBST）。具体来说，DMN学习用户自由修改的mask和目标图像之间的映射，实现多种生成结果。 EBST在源mask上对用户编辑行为进行建模，从而使整个框架对各种操纵的输入更加健壮。具体来说，它引入了dual-editing consistency作为辅助监督。
为便于进行广泛的研究，还构建了一个名为CelebAMask-HQ的细粒度mask的、大规模高分辨率数据集。
这个工作的主要idea是用一个叫做DMN的网络，把人脸mask和人脸对应起来，也就是可以很好地从人脸mask映射到真实人脸图像。然后对人脸mask进行编辑，在通过DMN就得到与之对应的编辑人脸。
![image](https://user-images.githubusercontent.com/36876387/134147449-c67b26b2-ba38-4989-a507-5e283fa11d30.png)

4.Interpreting the Latent Space of GANs for Semantic Face Editing

作者 | Yujun Shen, Jinjin Gu, Xiaoou Tang, Bolei Zhou
代码 | https://github.com/genforce/interfacegan
论文 | https://arxiv.org/abs/1907.10786
单位 | 香港中文大学，香港中文大学（深圳）
对GAN如何将从随机分布中采样的潜码映射到真实图像仍缺乏足够的了解。
在这项工作中，提出了一个称为InterFaceGAN的新颖框架，用于通过解释GAN所学到的潜在语义来进行人脸编辑。
作者发现，训练好的生成模型的潜码实际上在线性变换后即可学到解纠缠的表示。作者探索了各种语义之间的纠缠现象，并尝试对人脸属性进行更精确控制生成。
![image](https://user-images.githubusercontent.com/36876387/134151971-9bb058d4-20e4-4df7-a863-0f43729e7695.png)

5.CONFIG: Controllable Neural Face Image Generation

作者 | Marek Kowalski, Stephan J. Garbin, Virginia Estellers, Tadas Baltrušaitis, Matthew Johnson, Jamie Shotton
单位 | 微软
论文 | https://arxiv.org/abs/2005.02671
代码 | https://github.com/microsoft/ConfigNet
ConfigNet在真实面部图像和合成面部渲染上进行训练，该方法使用合成数据将潜在空间分解为与传统渲染pipeline的输入相对应的元素，从而将头部姿势、面部神情、发型和光照等诸多方面分解。 最后研究者提出了一种使用属性检测网络与用户研究相结合的评估标准，并实现了对输出图像属性的SOTA单独控制。
![image](https://user-images.githubusercontent.com/36876387/134148447-02c4f13c-69d0-424c-9fb9-b6c86b67e34b.png)


6.CAFE-GAN: Arbitrary Face Attribute Editing with Complementary Attention Feature

作者 | Jeong gi Kwak, David K. Han, Hanseok Ko
单位 | 高丽大学；ARL
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123590511.pdf
面部属性编辑的目的是根据给定的目标属性（例如，头发的颜色，胡须，性别等）更改面部图像。已经有一些工作集中在利用对抗性生成网络（GAN）进行面部属性编辑。这些方法已取得了一些成功，但它们也导致面部区域意外变化，这意味着生成器会更改与指定属性无关的区域。为了解决这个意想不到的变化问题，提出了一种新颖的GAN模型，该模型通过补充注意特征Complementary attention feature(CAFE)的仅编辑与目标属性相关的面部部分。
![image](https://user-images.githubusercontent.com/36876387/134148468-0ca0704f-1115-4fcd-814f-65a459831c11.png)

7.CooGAN: A Memory-Efficient Framework for High-Resolution Facial Attribute Editing

作者 | Xuanhong Chen, Bingbing Ni, Naiyuan Liu, Ziang Liu, Yiliu Jiang, Loc Truong, Qi Tian
单位 | 上海交通大学；Huawei HiSilicon；华为
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560647.pdf
代码 | https://github.com/XHChen0528/CooGAN
人脸属性编辑
![image](https://user-images.githubusercontent.com/36876387/134148493-1bd83d56-5b7b-44b8-95a6-3176f98f7438.png)

8.SSCGAN: Facial Attribute Editing via Style Skip Connections
作者 | Wenqing Chu, Ying Tai, Chengjie Wang, Jilin Li, Feiyue Huang, Rongrong Ji
单位 | 腾讯优图；厦门大学
论文 | https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123600409.pdf
通过编辑表示样式特征的通道全局信息来执行属性传递。开发了一种基于跳过样式连接的生成对抗网络，可实现精确的面部属性操纵。
问题：现有的人脸属性编辑方法通常采用编码器-解码器结构，其中属性信息被表达成一个one-hot向量然后与图像或特征层拼接起来。然而，这样的操作只学到了局部的语义映射而忽略了全局的人脸统计信息。
方法：本文提出通过修改通道层面的全局信息(风格特征)来解决上述问题。设计了一个基于风格跳跃连接的生成对抗网络(SSCGAN)来实现精准的人脸属性操纵。具体来说，在编码器和解码器之间的多个风格跳跃连接路径上注入目标属性信息，每个连接会抽取编码器中的隐藏层的风格特征，然后做一个基于残差的映射函数来将这个风格特征迁移到目标属性的空间。接下来，这个被调整过的风格特征可以用作输入来对解码器的隐藏层特征做实例归一化。此外，为了避免空间信息的损失(比如头发纹理或瞳孔位置)，进一步引入了基于跳跃连接的空间信息传递模块。
![image](https://user-images.githubusercontent.com/36876387/134151904-0c132e77-d66d-47cf-9bda-3140e5e25bb1.png)

9.Toward Fine-grained Facial Expression Manipulation

作者 | Jun Ling, Han Xue, Li Song, Shuhui Yang, Rong Xie, Xiao Gu
单位 | 上海交通大学
论文 | https://arxiv.org/abs/2004.03132
代码 | https://github.com/junleen/Expression-manipulato
问题：面部表情操纵旨在在给定条件下编辑面部表情。之前的方法可能会遇到与条件无关的区域发生更改的情况，或者无法进行细粒度的编辑。
方法：考虑到这两个目标，提出了一种新颖的方法。首先，将连续绝对条件替换为相对条件，特别是相对动作单位。利用相对动作单位，生成器学习仅变换由非零值相对AU指定的感兴趣区域。其次，生成器基于U-Net构建，通过多尺度特征融合（MSF）机制进行了增强，可实现高质量的表达式编辑目的。
![image](https://user-images.githubusercontent.com/36876387/134148597-d5c8b5c4-f6a9-4d3c-98b8-074a9a5e584e.png)


10.Learning Formation of Physically-Based Face Attributes
作者 | Ruilong Li, Karl Bladin, Yajie Zhao, Chinmay Chinara, Owen Ingraham, Pengda Xiang, Xinglei Ren, Pratusha Prasad, Bipin Kishore, Jun Xing, Hao Li
单位 | USC Institute for Creative Technologies，南加州大学，Pinscreen
论文 | https://arxiv.org/abs/2004.03458
进行id和表情的解缠，提供低维特征向量控制面部
![image](https://user-images.githubusercontent.com/36876387/134149516-155cd8e4-05f9-4f77-845e-102e7f4f79ed.png)


11.FaceScape: A Large-Scale High Quality 3D Face Dataset and Detailed Riggable 3D Face Prediction

作者 | Haotian Yang, Hao Zhu, Yanru Wang, Mingkai Huang, Qiu Shen, Ruigang Yang, Xun Cao
代码 | https://github.com/zhuhao-nju/facescape
该论文发布大尺度高精度人脸三维模型数据库FaceScape，并首次提出从单幅图像预测高精度、可操控人脸三维模型的方法。FaceScape数据库包含约18000个高精度三维面部模型，每个模型包含基底模型和4K分辨率的置换图及纹理贴图，能够表征出面部极细微的三维结构和纹理。与现有公开的三维人脸数据库相比，FaceScape在模型数量和质量上均处于世界最高水准。
在FaceScape数据库的基础之上，本文还探索了一项具有挑战性的新课题：以单幅人脸图像为输入，预测高精度、表情可操控的三维人脸模型。该方法的预测结果能够通过表情操控生成精细的面部模型序列，所生成的模型在新表情下仍然包含逼真的细节三维结构。据悉，FaceScape数据库和代码将于近期免费发布，供非商业用途的学术研究使用。
![image](https://user-images.githubusercontent.com/36876387/134149633-8471ab97-e970-4667-93b4-4f70a046143d.png)

12.Adversarial Latent Autoencoders
作者 | Stanislav Pidhorskyi, Donald Adjeroh, Gianfranco Doretto
论文 | https://arxiv.org/abs/2004.03132
代码 | https://github.com/podgorskiy/ALAE
本文提出的Adversarial Latent Autoencoder (ALAE)是一种结合了自编码器、更具通用性的、利用GAN方法的架构，它可以进行更“解耦”的表征学习。
ALAE不仅可以生成可以和StyleGAN媲美的1024大图，还可以对真实image进行更好的重建、编辑等。
![image](https://user-images.githubusercontent.com/36876387/134149666-d1d05e4c-1b3f-4d48-8107-0f0c517a280f.png)
![image](https://user-images.githubusercontent.com/36876387/134149690-cab1bc0c-efc2-4890-9259-b264635f94f0.png)

13.StyleRig: Rigging StyleGAN for 3D Control over Portrait Images
论文 | https://arxiv.org/pdf/2004.00121.pdf
StyleGAN可以生成具有极具真实感的肖像图像，但缺乏对3D可解释的语义参数（如脸部姿势，表情，和场景照明）。
3DMM提供了语义参数以控制，但是在渲染时缺乏真实感，且仅对人脸进行建模，而对肖像其他部分（头发、嘴部内部、背景）不进行建模。
本文提出通过3DMM对预训练、固定的StyleGAN进行面部语义参数控制的方法；方法以自监督式训练，无需人工标注
![image](https://user-images.githubusercontent.com/36876387/134149732-6a4d5bc5-441d-4516-b5b0-b4cecddfb093.png)


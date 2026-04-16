很抱歉，暂时只支持 M 系列的苹果系统

需要自己准备一个支持图片分析的 LLM 大模型，多数多模态的都支持

##谨防不支持图片的大模型出现幻觉乱分析

更新了几版后，目前这个算勉强能用了

_找个机会 B 站录个教学视频_

不再支持FTP批量上传，因为如果不是一两百的上传数量，普通人几十条上传的那种，应该还是官方的[上传页面](https://www.pond5.com/zh/index.php?page=my_uploads)更好用。

当前这个版本只支持将素材解析了之后生成对应的CSV文件，帮助大家解决最繁琐的标题描述以及打标签环节。
可以使用后台的[「应用CSV」](https://www.pond5.com/zh/index.php?page=apply_csv)页面进行一键绑定匹配。

希望能帮大家节省点时间出来玩手机或者睡觉......

**关于[ CSV 页面](https://www.pond5.com/zh/index.php?page=apply_csv)的选项**

Limit to clips...
「请选择 That need to be tagged」

- [ ] 四个要勾的选项都请勾上
- [ ] 2
- [ ] 3
- [ ] 4

日期格式
yyyy-mm-dd _（就是年月日如 2026-04-16，一般这个在我在粗剪导出要上传的素材的时候，重新命名都是这样命名的，这里根据自己的习惯选）_

Command
「请选择 Apply CSV to clips」

_提交后若出现不理解的错误，或者对提交后的内容有不理解的，建议直接复制发给 ai 帮你解析（我也是这么干的）_

**关于解析的大模型的选择与使用**
中间帧、首尾帧是用本地的脚本抽取的，不消耗token；
图像分析需要调用大模型的算力运行，可以是本地的，也可以是云端的；
个人建议新用户先用各个大厂免费的新用户算力，比如火山引擎（字节家）每个大模型会送五十万 token，分析个一两百张应该没问题，各家都试用过后，再决定买哪家的云端大模型算力，就是 coding plan；
如果电脑性能好的，也可以在本地部署大模型，只是解析图片的话，一般 3080 12G 显存都没问题，我是 mac mini4 也能凑合跑，但是因为我本身就有定阅 coding plan 来做自己的小玩意儿（比如现在的这个），所以我用云端的来跑。

<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/00999e89-c414-4b63-82ce-a9d934b99ce1" />
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/663c1162-79bb-4606-a644-584a7dd2f850" />
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/56124c99-47b8-461a-9554-ca2decf078a7" />
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/2a506a99-fb8a-40cb-8af3-9b8d4b3faf69" />
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/c42768f7-30d2-4887-a1aa-b98c0c912371" />
<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/8962a35f-97a1-4f52-9371-8826ebd2618c" />

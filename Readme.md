

This is a production-grade, state-of-the-art (SOTA) result achieved under strict engineering constraints, ranking at the world-class tier for single-epoch training.

AUC 0.8085 : world-class, production-grade, achieved under time-based split (Day) within one epoch without fixed random seed..

<br>
<br>
No PyTorch, No TensorFlow, No third-party librarie

Lightweight, low-memory C++ implementation

Only C++ header file.
<br>
<br>
criteo 45M datasets (7:2:1) or (9:1).

<br>
<br>
Remark and Note ：

  Test is on One Epoch and Time-split (Day1-5 -> Day7/ Day1-4 -> Day6) or (Day1-6 -> Day7/Day1-5 - > Day6) and  No Best Selection and No    Cumulative Features and No fixed random seed.

工业工程级测试标准：

  1. 按FuxiCTR 方式训练测试 one epoch AUC 0.8055 （FuxiCtr AUC 看下图，感觉有问题）

  2. 按google 方式训练测试 one epoch AUC 0.8085    （google AUC 0.8099 实验环境 ，非 day by day 即没有按天时序测试 ，如 ，按工业工程级实际大概 0.8066）

  微调太费时间了，懒得优化了...

<br>

1. One Step of Test:

Testing : AUC 0.8055 (day1-4 -> day 6)

<img width="682" height="728" alt="图片" src="https://github.com/user-attachments/assets/b83c929b-8e4c-4761-a152-54b0f62f54be" />

Testing : AUC 0.8085 (day1-5 -> day 6 )

<img width="636" height="692" alt="图片" src="https://github.com/user-attachments/assets/67f12071-2b65-4c9c-9f67-f431da30ea83" />


<br>
<br>
开源SOTA FuxiCTR ，开启了Best模型的情况下
<br>
<img width="686" height="120" alt="图片" src="https://github.com/user-attachments/assets/166cabfe-0472-41bc-a39d-34a5315c5d23" />
<br>
<br>
有一些不太合理的地方。
<br>
1. 很多轮后 突然跳涨0.004 罕见
<img width="707" height="434" alt="图片" src="https://github.com/user-attachments/assets/eecd1a58-c60c-473e-85ff-ffb845951c1c" />
<br>
2. Test AUC > Validation AUC > Train AUC (罕见而且不合理)
<img width="1030" height="327" alt="图片" src="https://github.com/user-attachments/assets/a059cb57-cbfe-4b2d-a8aa-40a73afced34" />

<br>
<br>


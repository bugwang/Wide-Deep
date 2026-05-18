No Pytorch，No Tensorflow 

Only C++ header file.
criteo 45M datasets (7:2:1).

Remark and Note ：
Test is on One Epoch and Time-split (Day 1-5 -> Day 7) and  No Best Selection and No Cumulative Features

工业工程级测试标准。
<br>

1. One Step of Test:

Testing : AUC 0.8055

<img width="682" height="728" alt="图片" src="https://github.com/user-attachments/assets/b83c929b-8e4c-4761-a152-54b0f62f54be" />

<br>
<br>
开源SOTA FuxiCTR ，开启了Best模型的情况下
<br>
<img width="686" height="120" alt="图片" src="https://github.com/user-attachments/assets/166cabfe-0472-41bc-a39d-34a5315c5d23" />
<br>
<br>
有一些不太合理的地方。
1. 很多轮后 突然跳涨0.004 罕见
<img width="707" height="434" alt="图片" src="https://github.com/user-attachments/assets/eecd1a58-c60c-473e-85ff-ffb845951c1c" />
<br>
2. Test AUC > Validation AUC > Train AUC (罕见而且不合理)
<img width="1030" height="327" alt="图片" src="https://github.com/user-attachments/assets/a059cb57-cbfe-4b2d-a8aa-40a73afced34" />

<br>
<br>


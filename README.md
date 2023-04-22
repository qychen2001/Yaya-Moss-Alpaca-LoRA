# Yaya-Moss-Alpaca-LoRA

【丫丫】是以Moss作为基座模型，使用LoRA技术进行指令微调的尝试。由黄泓森，陈启源 @ 华中师范大学主要完成。同时它也是[【骆驼】开源中文大语言模型](https://github.com/LC1332/Luotuo-Chinese-LLM)的一个子项目，它由陈启源 @ 华中师范大学，李鲁鲁，冷子昂 @ 商汤科技 发起 。

**( 注意: [陈启源](https://qiyuan-chen.github.io/) 正在寻找2024推免导师; 黄泓森正在寻找运维/C++实习，欢迎进一步与我们联系 )**

我们将项目命名为 丫丫 主要是因为，Moss和丫丫都是电影《流浪地球》中的角色。

## 新闻

[2023-4-22] 我们已经完成了基于中文Alpaca数据的LoRA训练，已经放出训练代码、数据和评测脚本

[2023-4-21] 我们已经开始了基于中文Alpaca数据的LoRA训练

## 训练步骤

1. 我们是在两张A100 40G上完成的训练，如果你的显卡显存不足，可以尝试减小batch size，但至少应该有40G以上的显存用于训练。

2. 环境安装

   ```bash
   pip install -r requirements.txt
   ```

3. 开始训练！训练代码保存在`src/train.ipynb`中。

4. 我们训练好的LoRA模型已经上传至Huggingface，你可以在[这里](https://huggingface.co/silk-road/yaya-moss-alpaca-lora-0.1)下载使用。我们的评测代码在`src/evaluate.ipynb`中。

5. 更多的评测结果和分析正在整理中，敬请期待！

## 开源协议

为了和MOSS项目保持一致，本项目所含代码采用[Apache 2.0](https://github.com/qiyuan-chen/Yaya-Moss-Alpaca-LoRA/blob/main/LICENSE)协议，数据采用[CC BY-NC 4.0](https://github.com/qiyuan-chen/Yaya-Moss-Alpaca-LoRA/blob/main/DATA_LICENSE)协议，模型权重采用[GNU AGPL 3.0](https://github.com/qiyuan-chen/Yaya-Moss-Alpaca-LoRA/blob/main/MODEL_LICENSE)协议。

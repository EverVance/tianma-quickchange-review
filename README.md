# 天马座夹爪快换评审网页

状态：工作稿，正式版本待用户锁定。硬件框图以用户 2026-10-13 放入临时交换的版本为编辑基准。

- 入口：`index.html`；拆换动画：`motion.html`；可编辑框图：`hardware.drawio`。
- MCU、上游 CAN FD 收发器、电机 CAN FD 备选收发器独立画出。两组 H/L 0Ω 互斥选择上游直通或 MCU 控制；共用下游 CAN 双线通断开关。
- 固定侧保护壳、Board B 40×10 mm、结构动画及板框候选保持原内容。框图与页面修改不是 PCB 或机械加工验收。
- 两个旧版 GRIPPER_SENSOR 原理图/PCB 未因本次网页整理修改。
- 公开地址：https://evervance.github.io/tianma-quickchange-review/
- 此目录是当前网页的维护与发布源，保留完整 Git 历史。双击 index.html 可离线浏览；使用本地网页服务器时以此目录为根目录。
- Information 正式版本记录以用户锁定为准；内部提交和缓存时间戳不代表正式版本。

电机 CAN FD2 引脚依据：[ST STM32G0B1 数据手册](https://www.st.com/resource/en/datasheet/stm32g0b1cc.pdf)，PB0 RX / PB1 TX，AF3。CAN FD 收发器能力不代表电机协议和全链路速率已经验证。

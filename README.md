<div align="center">


![cover](assets/cover.png)

# task-queue-protocol

**高峰时段只入队不执行，闲时统一跑。**

<p>
  <a href="#"><img src="https://img.shields.io/badge/peak--hours-9-12%20%2F%2014-18-red" alt="Peak hours" /></a>
  <a href="#"><img src="https://img.shields.io/badge/off--peak-immediately-green" alt="Off-peak immediate" /></a>
</p>

[规则](#核心规则) · [判断逻辑](#判断逻辑)

</div>

---

## 核心规则

| 时段 | 收到任务怎么办 |
|------|--------------|
| 高峰 9-12 / 14-18 | 只入队，不执行，回复"已入队，闲时处理" |
| 非高峰 12-14 / 18-次日9 | 立即执行，不等固定批次 |
| 用户说"现在/立刻/紧急" | 不管几点都立即执行 |

## 判断逻辑

1. 收到请求先看当前时间
2. 高峰到达 → 入队，给预计窗口
3. 非高峰到达 → 直接做
4. 误执行高峰任务 → 标注"高峰期误执行"，不掩饰

## License

MIT

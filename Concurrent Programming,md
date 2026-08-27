# std::atomic
**原子（atomic）**：一个操作要么完整执行完，要么完全不执行，中间不会被其他线程打断。
整数 `int/unsigned long long`、指针、bool、浮点（C++20 起），游戏开发最常用 `atomic<bool>`、`atomic<uint32_t>`。
## 关键接口：
- `.load()`：原子读取值
- `.store(val)`：原子写入值
- `.fetch_add(x)` / `.fetch_sub(x)`：原子加减
- `.exchange(val)`：原子交换，返回旧值
## 选用准则（游戏引擎开发）
- 只是单个标记、计数器、状态 ID → 用`std::atomic`
- 保护容器、数组、复杂对象、多变量读写 → 用`std::mutex`
## 关键限制

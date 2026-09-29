# 🛡️ C语言网络安全进攻与防守字典

一个从**小白到大佬**的系统化学习路线，帮助初学者逐步掌握网络安全的进攻与防守技术。

## 📚 学习路线图

### 第一阶段：基础知识 (入门级)
掌握C语言基础和计算机底层概念

- [x] C语言基础回顾
  - 指针和内存管理
  - 数组和字符串
  - 函数调用和栈
  - 结构体和联合体

- [x] 计算机底层概念
  - 内存布局（栈、堆、数据段）
  - CPU寄存器和指令
  - 函数调用约定
  - 缓冲区的概念

### 第二阶段：常见漏洞 (初级)
理解最常见的安全漏洞原理

- [x] 缓冲区溢出 (Buffer Overflow)
  - 栈溢出 (Stack Overflow)
  - 堆溢出 (Heap Overflow)
  - 整数溢出 (Integer Overflow)

- [x] 格式化字符串漏洞 (Format String Vulnerability)
  - 信息泄露
  - 内存写入

- [x] 使用释放后漏洞 (Use-After-Free, UAF)
  - 原理和利用方法

- [x] 一二一漏洞入门级实践

### 第三阶段：进攻技术 (中级)
学习如何利用这些漏洞进行进攻

- [x] Shellcode基础
  - 编写简单的Shellcode
  - Shellcode编码和绕过

- [x] 栈溢出利用
  - 基于ROP的绕过
  - 控制程序流

- [x] 堆利用技术
  - 堆喷射
  - 堆块复用

- [x] 高级绕过技术
  - ASLR绕过
  - DEP/NX绕过
  - 符号执行基础

### 第四阶段：防守技术 (中级)
学习如何防御这些进攻

- [x] 编译器防护
  - StackCanary (栈金丝雀)
  - RELRO保护
  - PIE (位置无关代码)

- [x] 运行时防护
  - ASLR (地址空间随机化)
  - DEP/NX (数据执行保护)

- [x] 代码审计技巧
  - 静态分析
  - 动态分析

- [x] 安全编码实践
  - 输入验证
  - 边界检查
  - 内存安全

### 第五阶段：综合实战 (高级)
结合进攻和防守的实战项目

- [x] CTF挑战题解析
  - Pwn题目分类
  - 解题思路和技巧

- [x] 真实漏洞分析
  - CVE案例学习
  - 补丁对比分析

- [x] 工具链掌握
  - GDB调试
  - IDA逆向
  - 其他安全工具

- [x] 项目实战
  - 安全审计项目
  - 漏洞发现项目

## 🗂️ 目录结构

```
cybersecurity-c-dictionary/
├── README.md                          # 本文件
├── LEARNING_ROADMAP.md               # 详细学习路线
├── RESOURCES.md                      # 学习资源汇总
│
├── 01-Basics/                        # 第一阶段：基础知识
│   ├── 01-C语言基础/
│   ├── 02-计算机底层/
│   └── README.md
│
├── 02-Vulnerabilities/               # 第二阶段：常见漏洞
│   ├── 01-缓冲区溢出/
│   ├── 02-格式化字符串/
│   ├── 03-使用释放后漏洞/
│   ├── 04-其他漏洞/
│   └── README.md
│
├── 03-Attack/                        # 第三阶段：进攻技术
│   ├── 01-Shellcode/
│   ├── 02-栈溢出利用/
│   ├── 03-堆利用/
│   ├── 04-高级绕过/
│   └── README.md
│
├── 04-Defense/                       # 第四阶段：防守技术
│   ├── 01-编译器防护/
│   ├── 02-运行时防护/
│   ├── 03-代码审计/
│   ├── 04-安全编码/
│   └── README.md
│
├── 05-Practice/                      # 第五阶段：综合实战
│   ├── 01-CTF题解/
│   ├── 02-CVE分析/
│   ├── 03-工具使用/
│   └── README.md
│
└── Resources/                        # 学习资源
    ├── Tools/                        # 工具配置
    ├── References/                   # 参考资料
    └── Checklists/                   # 检查清单
```

## 🎯 学习建议

1. **循序渐进** - 从第一阶段开始，不要跳跃
2. **动手实践** - 每个示例都要亲自运行和修改
3. **深入理解** - 理解原理而不是死记硬背
4. **记录笔记** - 保持学习笔记和总结
5. **参与讨论** - 在Issues中讨论和提问

## 🔧 环境要求

- Linux系统 (推荐Ubuntu 20.04+)
- GCC编译器
- GDB调试器
- Python 3.x
- 其他工具根据章节需要

### 快速安装

```bash
# Ubuntu/Debian
sudo apt-get update
sudo apt-get install build-essential gdb python3 python3-pip

# 其他工具
pip3 install pwntools

# Peda (GDB增强)
git clone https://github.com/longld/peda.git ~/peda
echo "source ~/peda/peda.py" >> ~/.gdbinit
```

## 📖 如何使用本字典

1. **从README开始** - 理解整体框架
2. **按阶段学习** - 每个阶段有独立的README
3. **查看代码示例** - 每个概念都有注释详细的代码
4. **做练习题** - 每章末尾都有练习题
5. **参考资源** - 使用RESOURCES.md查找更多学习材料

## 📚 相关资源

- **书籍**
  - 《深入浅出密码学》
  - 《0day安全：软件漏洞分析技术》
  - 《Hacking：The Art of Exploitation》

- **在线平台**
  - HackTheBox
  - CTFlearn
  - Pwnable.kr
  - Pwnable.tw

- **工具**
  - GDB/PEDA
  - IDA Pro
  - Radare2
  - pwntools

## 🤝 贡献指南

欢迎提交Issue和Pull Request！

- 发现错误或有改进建议？提交Issue
- 想要添加新内容？提交PR
- 有更好的解释方式？分享你的想法

## 📝 许可证

MIT License

## 💬 联系方式

有问题？在Issues中讨论或联系维护者。

---

**最后更新**：2026年9月29日

**学习进度**：正在建设中... 🚀

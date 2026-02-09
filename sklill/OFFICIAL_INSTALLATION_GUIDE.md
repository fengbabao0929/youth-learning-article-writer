# Claude Code 官方安装指南

## 官方安装方法

根据 Anthropic 官方文档，Claude Code 可以通过以下几种方式安装：

### 方法1：通过 npm 安装（官方推荐）

```bash
# 安装 Claude Code CLI
npm install -g @anthropic-ai/claude-code

# 验证安装
claude --version

# 启动 Claude Code
claude
```

### 方法2：桌面版（预览阶段）
- 下载 Claude Code 桌面版应用
- 目前处于预览阶段，提供原生桌面界面

### 方法3：通过包管理器安装

**macOS (Homebrew):**
```bash
brew install claude-code
```

**Linux (Snap):**
```bash
sudo snap install claude-code
```

## 系统要求

- **Node.js**: 18+ 或 20+ LTS 版本
- **操作系统**: Windows 10+, macOS 10.15+, Linux
- **内存**: 至少 8GB RAM
- **存储**: 至少 1GB 可用空间

## 安装步骤详解

### 1. 安装 Node.js（如果未安装）

**Windows:**
```bash
# 下载 Node.js LTS 版本
# 访问: https://nodejs.org/
# 安装时选择 "Add to PATH" 选项
```

**验证 Node.js 安装:**
```bash
node --version
npm --version
```

### 2. 安装 Claude Code

```bash
# 全局安装 Claude Code
npm install -g @anthropic-ai/claude-code
```

### 3. 验证安装

```bash
# 检查版本
claude --version

# 查看帮助
claude --help
```

### 4. 首次使用

```bash
# 启动交互式会话
claude

# 或直接提问
claude "帮我写一个Python函数计算斐波那契数列"
```

## 功能特性

Claude Code 提供以下主要功能：

- ✅ **代码生成和补全** - 智能生成代码片段
- ✅ **代码解释** - 理解复杂代码逻辑
- ✅ **调试和修复** - 识别并修复代码问题
- ✅ **代码搜索** - 在代码库中搜索和理解代码
- ✅ **终端命令执行** - 执行 bash 命令
- ✅ **多语言支持** - Python, JavaScript, Java, C++, Go 等

## 配置和使用

### 基本配置

```bash
# 查看当前配置
claude --help

# 设置模型偏好
claude --model claude-3-sonnet

# 设置工作目录
cd /path/to/your/project
claude
```

### 常用命令示例

```bash
# 代码生成
claude "写一个React组件显示用户列表"

# 代码解释
claude "解释这段异步JavaScript代码的工作原理"

# 调试帮助
claude "帮我找出这个Python函数中的错误"

# 代码重构
claude "优化这个SQL查询的性能"
```

## 故障排除

### 常见问题

1. **命令未找到**
   ```bash
   # 检查 Node.js 是否安装
   node --version
   
   # 检查 npm 全局安装路径
   npm config get prefix
   
   # 将路径添加到环境变量
   export PATH=$PATH:$(npm config get prefix)/bin
   ```

2. **权限问题**
   ```bash
   # 在 macOS/Linux 上可能需要 sudo
   sudo npm install -g @anthropic-ai/claude-code
   
   # 或更改 npm 全局安装目录权限
   npm config set prefix ~/.npm-global
   ```

3. **网络连接问题**
   ```bash
   # 使用国内镜像源
   npm config set registry https://registry.npmmirror.com
   
   # 安装 Claude Code
   npm install -g @anthropic-ai/claude-code
   ```

## 更新和卸载

### 更新 Claude Code
```bash
npm update -g @anthropic-ai/claude-code
```

### 卸载 Claude Code
```bash
npm uninstall -g @anthropic-ai/claude-code
```

## 官方资源

- **官方网站**: https://www.anthropic.com
- **文档**: https://docs.anthropic.com
- **GitHub**: https://github.com/anthropics
- **社区支持**: Anthropic 官方论坛

---

*本指南基于 Anthropic 官方文档和最佳实践编写，建议定期查看官方文档获取最新信息。*
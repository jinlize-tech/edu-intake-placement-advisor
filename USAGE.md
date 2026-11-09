# 使用说明

## 适用任务

学生英语口语较好但语法基础薄弱，家长希望直接进入高阶班。

## 准备输入

学生年级、学习经历、测评结果、课程级别目标、可用时间、班型容量、家长偏好、教师观察。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认测评口径
2. 对照课程先修要求
3. 检查硬约束
4. 生成首选/备选班型
5. 说明风险
6. 设计衔接任务
7. 人工确认

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。

# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `student_profile` | 学生基本情况 | string | 是 |
| `assessment_results` | 测评结果 | array | 是 |
| `course_catalog` | 课程与级别 | array | 是 |
| `available_classes` | 可入班清单 | array | 是 |
| `schedule_constraints` | 时间约束 | array | 是 |
| `parent_preferences` | 家长偏好 | string | 否 |
| `capacity` | 容量规则 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `分班建议表`：结构化条目数组，不允许空壳或占位文本。
- `依据`：结构化条目数组，不允许空壳或占位文本。
- `硬约束冲突`：结构化条目数组，不允许空壳或占位文本。
- `备选路径`：结构化条目数组，不允许空壳或占位文本。
- `试读/过渡建议`：结构化条目数组，不允许空壳或占位文本。
- `待确认项`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。

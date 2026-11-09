# 入学测评与分班建议示例

## 典型场景

学生英语口语较好但语法基础薄弱，家长希望直接进入高阶班。

## 具体示例

系统建议先进入高阶班并配两周语法桥梁任务，同时说明直接跳级风险，不替机构作最终承诺。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "student_profile": "学生基本情况已核对（脱敏示例）",
  "assessment_results": [
    {}
  ],
  "course_catalog": [
    {}
  ],
  "available_classes": [
    {}
  ],
  "schedule_constraints": [
    {}
  ],
  "parent_preferences": "家长偏好已核对（脱敏示例）",
  "capacity": "容量规则已核对（脱敏示例）"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出分班建议表、依据、硬约束冲突等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。

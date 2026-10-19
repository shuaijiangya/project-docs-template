# 自动生成文档

此目录只存放能由代码、Schema 或工具确定性生成的内容。生成源是权威，生成结果用于阅读和评审。

| 文件 | 权威源 | 生成命令 | 生成器版本 | 是否提交 |
| --- | --- | --- | --- | --- |
| [db-schema.md](db-schema.md) | `{{SCHEMA_SOURCE_PATH}}` | `{{SCHEMA_GENERATE_COMMAND}}` | `{{VERSION}}` | `{{YES_OR_NO}}` |

复制模板后的第一步是配置真实生成器，然后覆盖示例文件。不得手工编辑生成内容；若输出不对，修复生成源或生成器，再重新生成。

CI 应运行生成命令并检查工作区是否产生未提交差异：`{{GENERATED_DOCS_VERIFY_COMMAND}}`。若项目没有数据库或不提交生成结果，可删除 `db-schema.md` 并调整本表。

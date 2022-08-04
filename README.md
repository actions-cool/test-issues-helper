# Test Actions

## Issues Helper

### 新开 issue 检查是否触发 welcome

- 加 emoji
- comment 回复
- assigned
- label `welcome1` `welcome2`
- 删除该 issue，确保下次可测试

### 新开 issue 输入标题官网挂了
2
- 查看是否触发校验
- 回复评论
- 关闭 issue

### 测试 label `help wanted` `🤔 Need Reproduce`

- 查看是否可以回复

### 测试 label `add-assignees-1` `add-assignees-2`

- 是否随机指定正常

### 测试 issus `mark-duplicate`

- 输入 `Duplicate of #xx`
- 查看是否新增 `duplicate`
- 查看是否自动关闭
- 查看是否移除 `status: needs triage` or `status: needs triage2`
- 查看是否会影响其他 label

### 测试 label `remove-labels`

- 测试是否可以移除 `x1` or `x2`

### ~测试 label `month-statistics`~

- 查看是否可以新增 issue 统计

### 测试 label `check-inactive`

- 是否原有 inactive 无操作
- 是否可以把打开的所有issue 增加 label
- 是否回复
- 是否增加 emoji

### ~更新 `incative` issue~

- 查看是否会移除 `incative` label

### 测试 label `close-issues`

- 是否可以把 `🤔 Need Reproduce` 的 issue 关闭
- 是否评论，是否增加 emoji

### 测试 label `lock-issue`

- 是否锁定 issue hot 原因

### 保留若干 issues

- 测试 🤔 Need Reproduce 是否 1 天非活跃关闭
- 测试 needs-more-info 是否 2 天非活跃关闭

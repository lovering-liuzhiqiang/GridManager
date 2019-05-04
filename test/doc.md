# 宽度调整功能
- `disableCache:false`
- 操作任意列宽度调整
- 刷新后，调整后的宽度被记忆
- 清除缓存后，恢复为初始状态

- `disableCache:true`
- 操作任意列宽度调整
- 刷新后，恢复为初始状态
- `disableCache:false`

# 位置拖拽功能
- `disableCache:false`
- 对任意列进行位置拖拽
- 刷新后，调整的位置被记忆
- 清除缓存后，恢复为初始状态

- `disableCache:true`
- 对任意列进行位置拖拽
- 刷新后，恢复为初始状态
- `disableCache:false`

# 显示隐藏功能
- `disableCache:false`
- 对任意两列进行隐藏
- 对其中一列再进行显示
- 刷新后，隐藏的那一列不显示
- 清除缓存后，恢复为初始状态

- `disableCache:true`
- 对任意两列进行隐藏
- 对其中一列再进行显示
- 刷新后，恢复为初始状态
- `disableCache:false`

# 排序功能
- `isCombSorting: false`
- 默认排序为: 创建时间=降序
- 点击最后修改时间排序按键，请求参数的排序字段为: 最后修改时间=降序
- 再次点击最后修改时间排序按键，请求参数的排序字段为: 最后修改时间=升序
- 刷新后，恢复为初始状态

- `isCombSorting: true`
- 默认排序为: 创建时间=降序
- 点击最后修改时间排序按键，请求参数的排序字段为: [创建时间=降序, 最后修改时间=降序]
- 再次点击最后修改时间排序按键，请求参数的排序字段为: [创建时间=降序, 最后修改时间=升序]
- 刷新后，恢复为初始状态
- `isCombSorting: false`

# 选择功能
- `useRadio: false, useRowCheck: false`
- 不可通过行进行选中，仅可以通过选择框进行选中
- 选择第1行后: 第1条为选中状态，全选框为半选状态，选中条数为1
- 选择第3行后: 第1和第3条为选中状态，全选框为半选状态，选中条数数为1
- 点击全选后: 当前页全部选中，全选框为选中状态，选中条数为当前页总条数.
- 再次点击全选后: 当前页全部未选中，全选框为未选中状态，选中条数为0
- 选择第1行后: 第1条为选中状态，全选框为半选状态，选中条数为1
- 跳转至第二页后: 选中条数为1，但是当前页没有显中状态的行
- 选择第1行后: 第1条为选中状态，全选框为半选状态，选中条数为2
- 通过getCheckedTr查看当前页选中的tr
- 通过getCheckedData查看当前两条数据正确
- 刷新后，恢复为初始状态

- `useRowCheck: true`
- 可通过行进行选中

- `useRadio: true, useRowCheck: false`
- 不可通过行进行选中，仅可以通过选择框进行选中
- 选择第1行后: 第1条为选中状态,选中条数为1
- 选择第2行后: 第2条为选中状态,选中条数为1
- 刷新后，恢复为初始状态

- `useRowCheck: true`
- 可通过行进行选中
- `useRadio: false, useRowCheck: false`

# 分页功能
- `disableCache:false`
- 页码跳转正常
- 上一页下一页跳转正常
- 切换显示条数，数据请求为切换后的条数
- 刷新后: 显示为刚才配置过的条数

- `disableCache:true`
- 切换显示条数，数据请求为切换后的条数
- 刷新后: 显示为初始条数
- `disableCache:false`

# 右键功能
- `supportMenu: true`
- 在区域内点击右键，可正常打开
- 右键功能可用
- `supportMenu: false`
- 在区域内点击右键，不能打开右键
- `supportMenu: true`

# 模板渲染及内部事件
- 模板解析正常
- 模板内事件可用

# 公开方法
- 公开方法全部可用

# 静态数据 `demo2`
- 数据可以展示完整
- destroy 执行正确
- init 执行正确
- reset data 执行正确

# 多表渲染 `demo3`
- 各表格语言显示正确
- 触发分页事件，对其它表无影响
- 触发排序事件，对其它表无影响
- 触发选择事件，对其它表无影响

# 通栏功能 `demo4`
- 通栏功能正常

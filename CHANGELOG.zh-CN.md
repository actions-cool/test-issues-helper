---
order: 6
title: 更新日志
toc: false
timeline: true
---

`antd` 严格遵循 [Semantic Versioning 2.0.0](http://semver.org/lang/zh-CN/) 语义化版本规范。

#### 发布周期

- 修订版本号：每周末会进行日常 bugfix 更新。（如果有紧急的 bugfix，则任何时候都可发布）
- 次版本号：每月发布一个带有新特性的向下兼容的版本。
- 主版本号：含有破坏性更新和新特性，不在发布周期内。

---

## 4.12.15

`2021-01-04`

🎉 新年快乐！

- 🐞 修复不兼容 less 4.0.0 的问题。
- 🐞 修复 Typography 可编辑态光标跳动的问题。[#28545](https://github.com/ant-design/ant-design/pull/28545)
- 🐞 修复 Tree 动态加载数据时重复点击展开节点会导致状态错误的问题。[#28349](https://github.com/ant-design/ant-design/issues/28349) [@liuchao233](https://github.com/react-component/tree/pull/401)
- 🐞 修复 TreeSelect & Select `searchValue` 在受控且有值时，下拉菜单无法打开的问题。[#28574](https://github.com/ant-design/ant-design/pull/28574)
- 🐞 修复 Dropdown 禁用菜单项内的链接样式。[#28578](https://github.com/ant-design/ant-design/pull/28578)
- 🐞 修复 Progress `steps` 显示精度问题。[#28530](https://github.com/ant-design/ant-design/pull/28530) [@gaoryrt](https://github.com/gaoryrt)
- 🐞 修复 Radio 在 Chrome 下的对齐样式问题。[#28616](https://github.com/ant-design/ant-design/pull/28616)
- 🐞 修复 Collapse 修改 `@collapse-header-padding` 时箭头位置不居中的问题。[#28507](https://github.com/ant-design/ant-design/pull/28507)
- 💄 优化 Card 图片白边样式。[#28624](https://github.com/ant-design/ant-design/pull/28624)
- Input
  - 🐞 修复 Input.TextArea 有 `maxLength` 时输入中文被截断的问题。[#28456](https://github.com/ant-design/ant-design/pull/28456)
  - 🆕 Input.TextArea 的 `showCount` 属性现在支持传入一个方法来自定义数字的展示格式了。[#28145](https://github.com/ant-design/ant-design/pull/28145) [@MrHeer](https://github.com/MrHeer)
  - 🆕 Input `focus` 支持配置获取焦点时的光标位置。[#28602](https://github.com/ant-design/ant-design/pull/28602)
- Modal
  - 🐞 修复 Modal 可以被拖拽到窗口外的问题。[#28438](https://github.com/ant-design/ant-design/pull/28527) [@mumiao](https://github.com/mumiao)
  - 🆕 Modal.method 新增 `afterClose` 回调，会在 Modal 完全关闭后触发。[#28053](https://github.com/ant-design/ant-design/pull/28053) [@liuchao233](https://github.com/liuchao233)
- Table
  - 🐞 修复 `childrenColumnName` 和 `checkStrictly={false}` 无法一起使用的问题。[#28568](https://github.com/ant-design/ant-design/pull/28568)
  - 🐞 修复 Checkbox.Group 内选择行为异常的问题。[#28576](https://github.com/ant-design/ant-design/pull/28576)
  - 🐞 修复无数据时固定表头样式错乱的问题。[#28323](https://github.com/ant-design/ant-design/issues/28323)
  - 🐞 修复自定义 `filterDropdown` 时 `onChange` 事件的 `filters` 参数总是接收空数组的问题。[#28627](https://github.com/ant-design/ant-design/pull/28627) [@Meowu](https://github.com/Meowu)
  - 🆕 新增 `expandable.columnWidth` 以自定义展开列的宽度。[#28249](https://github.com/ant-design/ant-design/pull/28249)
  - 🆕 选择项新增清空所有选项。[#28580](https://github.com/ant-design/ant-design/pull/28580) [@n0ruSh](https://github.com/ant-design/ant-design/pull/285)
- Image
  - 🐞 修复错位问题。[#28439](https://github.com/ant-design/ant-design/pull/28439) [@MoeCasts](https://github.com/MoeCasts)
  - 💄 添加预览样式。[#28235](https://github.com/ant-design/ant-design/pull/28235)
  - 🆕 支持使用鼠标滚轮缩放图片。[#react-component/image/52](https://github.com/react-component/image/pull/52) [@OmriGM](https://github.com/OmriGM)
  - 🆕 支持单独设置预览图片。[#react-component/image/56](https://github.com/react-component/image/pull/56) [@wangcch](https://github.com/wangcch)
- Upload
  - 🐞 修复不使用 `transformFile` 时也会有警告的问题。[#28455](https://github.com/ant-design/ant-design/pull/28455) [@YanYuanFE](https://github.com/YanYuanFE)
  - 🐞 修复 Upload 的 `fileList` 和 immer 数据配合使用报错问题。[#28636](https://github.com/ant-design/ant-design/pull/28636) [@mumiao](https://github.com/mumiao)
  - 🆕 Upload 新增 `maxCount` 属性以限制文件数量。[#28367](https://github.com/ant-design/ant-design/pull/28367)
- DatePicker
  - 🚀 优化 `disabledDate` 逻辑。[#react-component/picker/191](https://github.com/react-component/picker/pull/191)
  - 🆕 新增 `onKeyDown` 回调。[#react-component/picker/138](https://github.com/react-component/picker/pull/138) [@conquera99](https://github.com/react-component/picker/pull/138)
- Select
  - 🐞 修复 `options` 更新不会触发选择框内容更新的问题。[#react-component/select/580](https://github.com/react-component/select/pull/580) [@jameslahm](https://github.com/jameslahm)
  - 🐞 修复使用 `tagRender` 后点击选项无法打开下拉框的问题。[react-component/select/582](https://github.com/react-component/select/pull/582) [@mumiao](https://github.com/mumiao)
  - 🐞 修复 `tokenSeparators` 在中文输入法下无法正确识别分隔符的问题。[#28564](https://github.com/ant-design/ant-design/issues/28564)
  - 🆕 `ref` 新增 `scrollTo` 方法。[#react-component/select/565](https://github.com/react-component/select/pull/565)
  - 🆕 多选模式下 `maxTagCount` 支持 `responsive`。[#28520](https://github.com/ant-design/ant-design/pull/28520)
- 🆕 Slider 新增 range.draggableTrack 以支持范围刻度整体可拖拽。[#28592](https://github.com/ant-design/ant-design/pull/28592)
- 🆕 `message` 新增 `onClick` 回调，会在消息被点击时触发。[#28148](https://github.com/ant-design/ant-design/pull/28148) [@ZeroTo0ne](https://github.com/ant-design/ant-design/pull/28148)
- 🆕 Descriptions 上可以统一设置 `labelStyle` 和 `contentStyle`。 [#28613](https://github.com/ant-design/ant-design/pull/28613)
- 🆕 Form 的 `scrollToFirstError` 属性支持设置滚动的位置参数。[#28272](https://github.com/ant-design/ant-design/pull/28272) [@vouis](https://github.com/vouis)
- 🆕 Steps 新增 reponsive 属性用于关闭响应式样式。[#28459](https://github.com/ant-design/ant-design/pull/28459)
- 🌐 国际化
  - 🇭🇷 改进克罗地亚语的支持。[#28458](https://github.com/ant-design/ant-design/pull/28458)
- TypeScript
  - 🛠 修复 PageHeader 的 `title` 的类型问题。[#28374](https://github.com/ant-design/ant-design/pull/28374) [@zhukovvandrei](https://github.com/zhukovvandrei)
  - 🤖 修复 Carousel 中 `dontAnimate` 参数为可选类型。[#28090](https://github.com/ant-design/ant-design/pull/28090) [@jarretmoses](https://github.com/jarretmoses)

## 4.9.4

`2020-12-16`

- 🐞 Fix Menu delayed hover color transition in Chrome. [#28372](https://github.com/ant-design/ant-design/pull/28372)
- 🐞 Fix Tree node connection line position problem. [#28354](https://github.com/ant-design/ant-design/pull/28354) [@maksnester](https://github.com/maksnester)
- 💄 Fix Table fixed column `z-index` which makes Dropdown not showing on top. [#28346](https://github.com/ant-design/ant-design/pull/28346)
- TypeScript
  - 🤖 Fix `message.loading()` return type. [#28362](https://github.com/ant-design/ant-design/pull/28362)

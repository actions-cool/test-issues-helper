---
order: 6
title: Change Log
toc: false
timeline: true
---

`antd` strictly follows [Semantic Versioning 2.0.0](http://semver.org/).

#### Release Schedule

- Weekly release: patch version at the end of every week for routine bugfix (anytime for urgent bugfix).
- Monthly release: minor version at the end of every month for new features.
- Major version release is not included in this schedule for breaking change and new features.

---

## 4.12.15

`2021-01-04`

🎉 Happy New Year!

- 🐞 Fix the compatibility issue of less 4.0.0.
- 🐞 Fix the problem of cursor jumping when Typography is editable. [#28545](https://github.com/ant-design/ant-design/pull/28545)
- 🐞 Fix the problem that repeatedly clicking on expanded nodes when Tree dynamically loads data will lead to wrong status.[#28349](https://github.com/ant-design/ant-design/issues/28349) [@liuchao233](https://github.com/react-component/tree/pull/401)
- 🐞 Fix the problem that TreeSelect & Select cannot open the dropdown menu when it's `searchValue` has value. [#28574](https://github.com/ant-design/ant-design/pull/28574)
- 🐞 Fix Dropdown disabled menu item link style. [#28578](https://github.com/ant-design/ant-design/pull/28578)
- 🐞 Fix Progress `steps` display accuracy issue. [#28530](https://github.com/ant-design/ant-design/pull/28530) [@gaoryrt](https://github.com/gaoryrt)
- 🐞 Fix Radio align issue in Chrome. [#28616](https://github.com/ant-design/ant-design/pull/28616)
- 🐞 Fix Collapse arrow position not aligned when change @collapse-header-padding variable. [#28507](https://github.com/ant-design/ant-design/pull/28507)
- 💄 Optimize the white border style of Card images. [#28624](https://github.com/ant-design/ant-design/pull/28624)
- Input
  - 🐞 Fix TextArea value get cut when input chinese words. [#28456](https://github.com/ant-design/ant-design/pull/28456)
  - 🆕 The `showCount` property of Input.TextArea now supports passing in a method to customize the display format of the number. [#28145](https://github.com/ant-design/ant-design/pull/28145) [@MrHeer](https://github.com/MrHeer)
  - 🆕 Input `focus` supports configuring the cursor position when getting focus. [#28602](https://github.com/ant-design/ant-design/pull/28602)
- Modal
  - 🆕 Modal.method adds an `afterClose` callback that will be triggered after the Modal is completely closed. [#28053](https://github.com/ant-design/ant-design/pull/28053) [@liuchao233](https://github.com/liuchao233)
  - 🐞 Fix the problem that Modal can be dragged outside the viewport. [#28438](https://github.com/ant-design/ant-design/pull/28527) [@mumiao](https://github.com/mumiao)
- Table
  - 🐞 Fix the problem that Table childrenColumnName and checkStrictly={false} cannot be used together. [#28568](https://github.com/ant-design/ant-design/pull/28568)
  - 🐞 Fix Table selection abnormal behavior when inside Checkbox.Group. [#28576](https://github.com/ant-design/ant-design/pull/28576)
  - 🐞 Fix the problem that the sticky header style is messy when there is no data. [#28323](https://github.com/ant-design/ant-design/issues/28323)
  - 🐞 Fix the problem that `onChange` listener always receives empty list as `filters` parameter if use a custom `filterDropdown`. [#28627](https://github.com/ant-design/ant-design/pull/28627) [@Meowu](https://github.com/Meowu)
  - 🆕 Adds `expandable.columnWidth` to customize the width of the expanded column. [#28249](https://github.com/ant-design/ant-design/pull/28249)
  - 🆕 Adds clear all option from selection. [#28580](https://github.com/ant-design/ant-design/pull/28580) [@n0ruSh](https://github.com/ant-design/ant-design/pull/285)
- Image
  - 🐞 Fix the misalignment issue of Image component.[#28439](https://github.com/ant-design/ant-design/pull/28439) [@MoeCasts](https://github.com/MoeCasts)
  - 💄 Adds preview style. [#28235](https://github.com/ant-design/ant-design/pull/28235)
  - 🆕 Adds functionality for zoom in\out by sliding the wheel. [#react-component/image/52](https://github.com/react-component/image/pull/52) [@OmriGM](https://github.com/OmriGM)
  - 🆕 Support separate settings url for preview images. [#react-component/image/56](https://github.com/react-component/image/pull/56) [@wangcch](https://github.com/wangcch)
- Upload
  - 🐞 Fix a warning even when not using `transformFile`. [#28455](https://github.com/ant-design/ant-design/pull/28455) [@YanYuanFE](https://github.com/YanYuanFE)
  - 🐞 Fix Upload `fileList` cannot work with data that is produced by immer. [#28636](https://github.com/ant-design/ant-design/pull/28636) [@mumiao](https://github.com/mumiao)
  - 🆕 Upload adds a new `maxCount` property to limit the number of files. [#28367](https://github.com/ant-design/ant-design/pull/28367)
- DatePicker
  - 🚀 Optimize the logic of `disabledDate`. [#react-component/picker/191](https://github.com/react-component/picker/pull/191)
  - 🆕 Adds `onKeyDown` callback. [#react-component/picker/138](https://github.com/react-component/picker/pull/138) [@conquera99](https://github.com/react-component/picker/pull/138)
- Select
  - 🐞 Fix issue where `options` update does not trigger the selection box content update. [#react-component/select/580](https://github.com/react-component/select/pull/580) [@jameslahm](https://github.com/jameslahm)
  - 🐞 Fix the problem that the dropdown box cannot be opened after clicking the option with `tagRender`. [react-component/select/582](https://github.com/react-component/select/pull/582) [@mumiao](https://github.com/mumiao)
  - 🐞 Fix the problem that `tokenSeparators` can not recognize the separator correctly under Chinese input method. [#28564](https://github.com/ant-design/ant-design/issues/28564)
  - 🆕 Adds `scrollTo` to the `ref`. [#react-component/select/565](https://github.com/react-component/select/pull/565)
  - 🆕 `maxTagCount` supports `responsive` in `multiple` mode. [#28520](https://github.com/ant-design/ant-design/pull/28520)
- 🆕 Slider add a new `range.draggableTrack` prop. [#28592](https://github.com/ant-design/ant-design/pull/28592)
- 🆕 Descriptions support setting `labelStyle` & `contentStyle` directly. [#28613](https://github.com/ant-design/ant-design/pull/28613)
- 🆕 message added a new `onClick` callback that will be triggered when the message is clicked. [#28148](https://github.com/ant-design/ant-design/pull/28148) [@ZeroTo0ne](https://github.com/ant-design/ant-design/pull/28148)
- 🆕 The `scrollToFirstError` property of the Form adds support for setting the position for scrolling. [#28272](https://github.com/ant-design/ant-design/pull/28272) [@vouis](https://github.com/vouis)
- 🆕 Steps support reponsive which allows to turn off reponsive change. [#28459](https://github.com/ant-design/ant-design/pull/28459)
- 🌐 Localization
  - 🇭🇷 Improved Croatian language support. [#28458](https://github.com/ant-design/ant-design/pull/28458)
- TypeScript
  - ⚒️ Fix `title` type of PageHeader. [#28374](https://github.com/ant-design/ant-design/pull/28374) [@zhukovvandrei](https://github.com/zhukovvandrei)

## 4.9.4

`2020-12-16`

- 🐞 Fix Menu delayed hover color transition in Chrome. [#28372](https://github.com/ant-design/ant-design/pull/28372)
- 🐞 Fix Tree node connection line position problem. [#28354](https://github.com/ant-design/ant-design/pull/28354) [@maksnester](https://github.com/maksnester)
- 💄 Fix Table fixed column `z-index` which makes Dropdown not showing on top. [#28346](https://github.com/ant-design/ant-design/pull/28346)
- TypeScript
  - 🤖 Fix `message.loading()` return type. [#28362](https://github.com/ant-design/ant-design/pull/28362)

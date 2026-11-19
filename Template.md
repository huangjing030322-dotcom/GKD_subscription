# huangjing030322-dotcom 的 GKD 订阅

基于 [AIsouler/GKD_subscription](https://github.com/AIsouler/GKD_subscription) 的个人维护分支，保留原有规则并按个人使用需求补充更新。原项目已停止维护，本仓库的更新独立发布。

## 添加订阅

在 GKD 的「订阅」页面添加以下链接：

```txt
https://raw.githubusercontent.com/huangjing030322-dotcom/GKD_subscription/main/dist/AIsouler_gkd.json5
```

- 订阅名称：huangjing030322-dotcom 的 GKD 订阅
- 独立订阅 ID：20261119，与原作者订阅区分。
- 当前版本：v--VERSION--
- 当前包含 --APP_SIZE-- 个应用、--GROUP_SIZE-- 个应用规则组、--GLOBALGROUP_SIZE-- 个全局规则组。
- [适配应用列表](./dist/README.md) · [更新日志](./dist/CHANGELOG.md)

文件名沿用上游命名，以上链接中的仓库属于本人的 fork。请使用此链接获取本分支的更新。

## 使用说明

1. 安装并启用 [GKD](https://gkd.li/)，添加上方订阅链接。
2. 默认仅启用开屏广告类规则，其他规则按需手动开启。
3. 使用拷贝漫画时，开启该应用的「局部广告-卡片广告」规则组。
4. 仓库发布更新后，在 GKD 订阅页面下拉检查更新。

原作者订阅与本订阅包含大量相同规则，建议按需选择启用，避免重复执行。

## 本分支补充

- 拷贝漫画（`com.copymanga.app`）：在「局部广告-卡片广告」组新增关闭广告按钮规则。
- 匹配选择器：`ImageView[id="com.copymanga.app:id/ad_close"][desc="关闭"][clickable=true]`。
- 新规则已通过静态校验，实际效果以设备和应用版本为准。

## 维护与反馈

- [反馈问题](https://github.com/huangjing030322-dotcom/GKD_subscription/issues)时请提供应用版本、问题描述及 GKD 快照。
- 规则源码位于 `src/apps/`，修改后运行 `pnpm run check`、`pnpm run build` 生成订阅产物。
- [贡献指南](./CONTRIBUTING.md) · [选择器参考](./Selectors.md)
- 发布工作流支持手动运行，并在北京时间每日 03:00 检查规则变更后构建更新。Fork 的定时工作流需在 GitHub Actions 中启用后才会运行。

## 来源与声明

感谢 [AIsouler](https://github.com/AIsouler) 与原项目贡献者，以及 [gkd-kit/subscription](https://github.com/gkd-kit/subscription)。本仓库为个人维护分支，与原作者的维护状态及发布渠道相互独立。

沿用原项目声明：禁止在国内平台传播；仅供本人学习使用；精力有限，随缘更新。

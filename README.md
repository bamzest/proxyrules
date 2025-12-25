# ProxyRules

自动维护的代理规则集合，适用于 Clash 等代理工具。规则每日自动更新，聚合多个优质开源规则源。

## 简介

本仓库提供经过整理和分类的代理规则文件，存放在 `rules/` 目录下。规则通过 GitHub Actions 自动生成和更新，确保规则的时效性和准确性。

## 使用方法

直接引用本仓库中的规则文件到你的 Clash 配置中：

```YAML
rule-providers:
  ai:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bamzest/proxyrules/rules/rules/clash/ai.yaml"
    path: ./ruleset/ai.yaml
    interval: 86400
```

## 更新频率

规则每天 **22:00 UTC**（北京时间次日 06:00）自动更新。

## 规则来源

本仓库聚合了以下优质开源规则：

* [blackmatrix7/ios\_rule\_script](https://github.com/blackmatrix7/ios_rule_script)
* [ACL4SSR/ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)
* [LM-Firefly/Rules](https://github.com/LM-Firefly/Rules)

## 许可证

本项目采用 MIT 许可证。规则来源于各开源项目，遵循其各自的许可证。

## 相关链接

* [RuleRefinery](https://github.com/bamzest/rulerefinery) - 规则生成工具


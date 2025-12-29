# luci-lib
`git clone --recurse-submodules --depth=1 https://github.com/zoyo94/luci-lib.git`

# 包含这些玩意:
```bash
git submodule add -f --depth 1 https://github.com/QiuSimons/luci-app-daed.git luci-app-daed
git submodule add -f --depth 1 https://github.com/sbwml/luci-app-mosdns.git luci-app-mosdns
git submodule add -f --depth 1 https://github.com/gdy666/luci-app-lucky.git luci-app-lucky
git submodule add -f --depth 1 https://github.com/jerrykuku/luci-theme-argon.git luci-theme-argon
git submodule add -f --depth 1 https://github.com/jerrykuku/luci-app-argon-config.git luci-app-argon-config
git submodule add --force --depth 1 https://github.com/linkease/nas-packages-luci.git nas_luci  
git submodule add --force --depth 1 https://github.com/linkease/nas-packages.git nas 
git submodule add --force --depth 1 https://github.com/linkease/istore.git istore 
git submodule add -f --depth 1 https://github.com/destan19/OpenAppFilter.git   
git submodule add -f --depth 1 https://github.com/stevenjoezhang/luci-app-adguardhome.git  
```
#  添加子模块（不指定分支）

`git submodule add --force --depth 1 https://github.com/vernesong/OpenClash.git openclash`

# 进入子模块目录
`cd openclash`

# 设置远程跟踪分支并切换到dev
```bash
git config remote.origin.fetch "+refs/heads/dev:refs/remotes/origin/dev"
git fetch --depth=1 origin dev
git checkout -b dev origin/dev
```
# 通常我用的 opkg源
```
src/gz kiddin9 https://dl.openwrt.ai/packages-24.10/aarch64_generic/kiddin9
src/gz routing https://dl.openwrt.ai/packages-24.10/aarch64_generic/routing
src/gz packages https://dl.openwrt.ai/packages-24.10/aarch64_generic/packages
src/gz luci https://dl.openwrt.ai/packages-24.10/aarch64_generic/luci
src/gz base https://dl.openwrt.ai/packages-24.10/aarch64_generic/base
src/gz base2 https://mirror-03.infra.openwrt.org/releases/23.05.0/packages/aarch64_generic/base
src/gz Openwrt_luci https://op.dllkids.xyz/packages/aarch64_generic
```

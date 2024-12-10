# Comfyui更新说明

## 更新方法
```shell
# 从上游仓库获取最新更新
git fetch upstream
# 将上游的更改合并到你的本地分支，可能需要解决冲突
git merge upstream/master
# 如果你想要合并上游的其他分支（例如 feature-branch），可以直接使用 git merge：
git merge upstream/feature-branch

# 将合并后的代码推送到你的 fork 仓库
git push

# 合并所有标签，下面的命令将所有的标签从 upstream 添加到本地仓库
git fetch upstream --tags

# 推送到当前仓库到origin远程仓库
git push origin --all   # 推送所有分支
git push origin --tags  # 推送所有标签

# 如果想要回退git merge的代码
git reset --hard commit_id

```

## 20240910
1. 更新comfyui master到20240910 => 0.2.2+
2. 更新插件 
cg-use-everywhere
ComfyUI-Advanced-ControlNet
ComfyUI-Impact-Pack
3. 更新库
spandrel

## 20241024
1. 兼容本地工程需要的修改（修改处都注释了KEEN）
   修改点包括：load_image字段, import导入因app路径冲突
   修改文件： nodes.py、server.py、internal_routes.py

## 20241025
1. 同步comfyui master到20241025 => 0.2.4+

## 20241202
1. 同步comfyui master到 20241202 => 0.3.6

## 20241210
1. 同步comfyui master到 20241210 => 0.3.7+

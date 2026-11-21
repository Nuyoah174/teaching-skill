# teaching-skill

a habit of teaching

本仓库保存一套可复用的教学方法，供老师、协作者或其他 agent 接手时使用。权威版本是默认分支 `main` 上的文件。某次修改在合并进入 `main` 之前，只属于对应拉取请求里的待采用版本；交付时要说明它有没有合并。未合并的文本不是 `main` 上的正式版。

## 两份文件各自做什么

- [TEACHING_GUIDELINES.md](TEACHING_GUIDELINES.md) 是唯一的完整规范正文。带课、安排学习、验收和更新偏好，都按这份正文执行。`main` 上的这篇才是权威版本：[教学规范](https://github.com/Nuyoah174/teaching-skill/blob/main/TEACHING_GUIDELINES.md)。
- [skills/course-driven-learning/SKILL.md](skills/course-driven-learning/SKILL.md) 是技能入口，只保留交接时先抓住的要点。`main` 上的入口是 [技能入口](https://github.com/Nuyoah174/teaching-skill/blob/main/skills/course-driven-learning/SKILL.md)。

技能入口中的相对链接是 [../../TEACHING_GUIDELINES.md](TEACHING_GUIDELINES.md)，从 `skills/course-driven-learning/SKILL.md` 指回仓库根目录的规范正文。把这个入口交给新的 agent 之后，仍要明确要求它读取 `main` 上的最新完整规范。把入口交给 agent 不会自动同步或自动安装这些文件，也不能默认每一个 bot 都会自己去读。

## 可复制的接手指令

把下面整段交给准备接手的 agent：

```text
请先读取下面两份文件在默认分支 main 上的最新内容，再结合我当前的能力档案和现有计划接手。档案和计划里已经写过的信息不要重复询问，也不要重置已有进度。

- 技能入口：https://github.com/Nuyoah174/teaching-skill/blob/main/skills/course-driven-learning/SKILL.md
- 规范正文：https://github.com/Nuyoah174/teaching-skill/blob/main/TEACHING_GUIDELINES.md

规范正文以 main 上的最新完整版本为准。只拿到技能入口时，完整规范正文仍要单独读取。若无法读取，请直接说明没有读到，不要假装已经读过，也不要索要访问令牌。
```

## 如何读取

仓库是否公开，以 GitHub 上的实际设置为准。这篇说明不改变可见性。

- 若仓库是私有的，读取者需要已经拥有该仓库的读取权限。
- 若仓库是公开的，可以直接打开上面的地址；agent 还要自己具备通过网络读取该地址的能力。
- 无论仓库是私有还是公开，都不要向用户索要访问令牌。
- 没有读取权限时，由用户提供已经下载的最新 `SKILL.md` 和 `TEACHING_GUIDELINES.md`。单独一份 `SKILL.md` 只是摘要入口，不代表完整规范正文已经拿到。
- 使用离线副本时，注明该副本正文开头写明的版本和日期。离线副本不能被说成已经自动获得仓库里的最新版本。

## 以后如何更新规范

1. 先读取默认分支 `main` 上 [TEACHING_GUIDELINES.md](https://github.com/Nuyoah174/teaching-skill/blob/main/TEACHING_GUIDELINES.md) 的最新版本，并记下该版本的提交 SHA。
2. 只合并本次明确提出的新偏好。与旧文冲突时先处理冲突，再提交，不要整篇覆盖。
3. 在规范的变更记录里写明改了什么、为何改、日期。
4. 提交后核对仓库中的文件内容，并交付本次提交链接。
5. 若尚未合并进 `main`，明确说明当前状态。未合并的版本不是 `main` 上的正式版。

具体课表、进度、学习者身份与环境信息不写入本说明，也不写入规范正文。

# AWESOME 列表

## 编程语言 AWESOME 列表

| 语言                               | README                                                        | 总数   |
| :----------------------------------- | :------------------------------------------------------------ | :----- |
| [Python](https://a.x-cmd.com/python) | [README](https://github.com/edwinjhlee/awesome/lang/python)   | 100    |
| [Deno](https://a.x-cmd.com/deno)     | [README](https://github.com/edwinjhlee/awesome/lang/deno)     | 100    |
| [Node](https://a.x-cmd.com/node)     | [README](https://github.com/edwinjhlee/awesome/lang/node)     | 100    |
| [Bun](https://a.x-cmd.com/bun)       | [README](https://github.com/edwinjhlee/awesome/lang/bun)      | 100    |
| [Java](https://a.x-cmd.com/java)     | [README](https://github.com/edwinjhlee/awesome/lang/java)     | 100    |
| [Kotlin](https://a.x-cmd.com/kotlin) | [README](https://github.com/edwinjhlee/awesome/lang/kotlin)   | 100    |

## 贡献代码前必读

欢迎贡献你认为优秀的开源库！ 你只需要提交所推荐的库的元信息文件，这个文件以 YML 格式组织。

### Library 元信息组织方式

以 Go 生态的 `github.com/urfave/cli` 为例，说明如何组织 Library 的元信息文件。

1.  **确定库的唯一标识符：** `github.com/urfave/cli` 定义了托管网站 (一般为 github.com)，用户名 (urfave)，以及库名 (cli)。
2.  **确定库的分类：**  这个库归类为 `cli`。
3.  **确定元信息文件路径：** 关于这个库的信息将存放在 `lang/go/cli/cli-[urfave].yml` 这个文件。
    *   **格式：** `lang/<语言>/<分类, 可能有多层>/<库名>-[<用户名>].yml`
    *   **非 GitHub 托管：** 如果用户不是注册在 github.com，例如 codeberg.org，那么名称则是 `lang/go/cli/cli-[urfave][codeberg.org].yml`

### 库的 YML 文件格式

YML 格式很简单，仅包含 KEY: VALUE 对。 同样以 `urfave/cli` 为例：

```yml
name: cli
repo: github.com/urfave/cli
desc: A simple, fast, and fun package for building command line apps in Go
desc-zh:  # 可选：描述的中文翻译。 如果您无法提供，请留空。
```

### 内容不确定怎么办？ 大胆提交！

你可能不确定内容描述，或者不确定分类。 没关系，大胆按照你认为最好的形式贡献并提交。 AWESOME 并不是一个代码库，因此我们的管理非常宽松。 管理员可以先合并，后面马上进行修改；当然，如果贡献内容值得商榷，我们也可以在 PR 过程中沟通。 因此，不用担忧，请尽管提交你心仪的库！

即使合并之后，你仍可以就该项内容发 ISSUE 或者 Discussion 进行讨论。

## 贡献方式

我们推荐以下三种贡献方式：

1.  **直接通过 GitHub 网站界面提交 PR** - 适合提交新的库，或者修改库的描述。
2.  **通过标准 PR 流程贡献** - 适合更复杂的修改，例如重新调整库的分类。
3.  **通过 Issues 贡献** - 如果你不确定如何创建 pull request。

### 1. 通过 GitHub 网站界面提交 PR

此方法非常适用于小型贡献：

1.  **登录：** 确保您已登录到您的 GitHub 帐户。
2.  **创建新文件：**
    *   点击 "Add file" -> "Create new file"。
    *   如果您尚未 fork 该存储库到您的帐户，系统将提示您 fork。
3.  **编写库的信息文件**
    *   文件名将为 `cli-[urfave].yml`。
    *   参考上文的 YML 内容格式，填写。
4.  **提交更改：** 使用描述性消息提交新文件。
5.  **创建 Pull Request：**
    *   转到 [https://github.com/edwinjhlee/awesome/pulls](https://github.com/edwinjhlee/awesome/pulls) 并点击 "New pull request"。
    *   选择您 fork 的存储库中包含您的更改的分支。
    *   为您的 pull request 添加清晰的标题和描述。

维护人员将审查您的 pull request，并在必要时提供反馈，如果符合标准，则会合并它。

### 2. 通过标准 PR 流程贡献

此方法更适合于较大的贡献，例如重新调整库的分类，或者如果您喜欢使用本地开发环境。

**步骤 1：Fork 和克隆**

1.  将此存储库 fork 到您的 GitHub 帐户。
2.  将 fork 的存储库克隆到您的本地计算机：

```bash
git clone https://github.com/<your-username>/awesome.git
cd awesome
```

**步骤 2：创建新文件并添加内容**

1.  **文件位置：** 在 `lang` 目录中相应的类别目录中创建一个新的 YAML 文件。
    *   **示例：** 对于 `github.com/urfave/cli`（Go 库，类别：`cli`），文件路径将为 `lang/go/cli/cli-[urfave].yml`。
    *   **对于 codeberg.org：** 如果存储库托管在 codeberg.org 上，请在文件名中包含 `[codeberg.org]`：`cli-[urfave][codeberg.org].yml`

2.  **文件内容：** 使用以下 YAML 格式：

    ```yaml
    name: urfave/cli
    repo: github.com/urfave/cli
    desc: A simple, fast, and fun package for building command line apps in Go
    desc-zh:  # 可选：描述的中文翻译。 如果您无法提供，请留空。
    ```

**步骤 3：提交并推送更改**

1.  将新文件添加到您的 Git 存储库：

    ```bash
    git add lang/go/cli/cli-[urfave].yml
    ```

2.  使用描述性消息提交您的更改：

    ```bash
    git commit -m "Add urfave/cli to awesome-go (cli category)"
    ```

3.  将您的更改推送到您 fork 的存储库：

    ```bash
    git push origin main
    ```

**步骤 4：创建 Pull Request**

1.  转到 GitHub 上您 fork 的存储库。
2.  点击 "Contribute" 按钮，然后点击 "Open pull request"。
3.  确保基本存储库是 `edwinjhlee/awesome`，并且比较分支是您的分支。
4.  为您的 pull request 添加清晰的标题和描述。

**[可选] 步骤 5：在本地查看结果**

如果您安装了 [x-cmd](https://x-cmd.com)，您可以在提交 pull request 之前预览生成的 README 文件：

```bash
x ws gen go
```

这将生成 `go/README.md` 文件，允许您查看您的更改。

### 3. 通过 Issues 贡献

如果您不确定如何创建 pull request，您可以通过创建 issue 来建议新的库。
虽然这是最简单的方法，但强烈建议通过 pull request 贡献。请参考上面的步骤和演示。

另外, 如果你在 PR 过程中遇到问题, 可以加入 x-cmd 的用户群寻求协助。

[TODO: add 微信群和TG群的照片]

**发起 Issue 步骤**

1.  在此处创建一个新的 issue [here](https://github.com/edwinjhlee/awsome/issues) 并选择 "[new library]" 模板。
2.  填写包含存储库名称和简短描述的表单。


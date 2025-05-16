# Awesome Lists

## 💻 Programming Language AWESOME Lists

| Language                               | README                                                        | Total |
| :----------------------------------- | :------------------------------------------------------------ | :---- |
| [Python](https://a.x-cmd.com/python) | [README](https://github.com/edwinjhlee/awesome/lang/python)   | 100   |
| [Deno](https://a.x-cmd.com/deno)     | [README](https://github.com/edwinjhlee/awesome/lang/deno)     | 100   |
| [Node](https://a.x-cmd.com/node)     | [README](https://github.com/edwinjhlee/awesome/lang/node)     | 100   |
| [Bun](https://a.x-cmd.com/bun)       | [README](https://github.com/edwinjhlee/awesome/lang/bun)      | 100   |
| [Java](https://a.x-cmd.com/java)     | [README](https://github.com/edwinjhlee/awesome/lang/java)     | 100   |
| [Kotlin](https://a.x-cmd.com/kotlin) | [README](https://github.com/edwinjhlee/awesome/lang/kotlin)   | 100   |

## 📖 Required Reading Before Contributing Code

Contributions of excellent open-source libraries are welcome! You only need to submit the meta-information file of the recommended library, which is organized in YML format.

### Library Meta-Information Organization Method

Using `github.com/urfave/cli` from the Go ecosystem as an example, this explains how to organize the library's meta-information file.

1.  **Determine the unique identifier of the library:** `github.com/urfave/cli` defines the hosting website (usually github.com), username (urfave), and library name (cli).
2.  **Determine the library's category:** This library is categorized as `cli`.
3.  **Determine the meta-information file path:** Information about this library will be stored in the `lang/go/cli/cli-[urfave].yml` file.
    *   **Format:** `lang/<language>/<category, possibly multi-layered>/<library name>-[<username>].yml`
    *   **Non-GitHub Hosting:** If the user is not registered on github.com, for example, codeberg.org, then the name is `lang/go/cli/cli-[urfave][codeberg.org].yml`

### Library YML File Format

The YML format is very simple, containing only KEY: VALUE pairs. Using `urfave/cli` as an example again:

```yml
name: cli
repo: github.com/urfave/cli
desc: A simple, fast, and fun package for building command line apps in Go
desc-zh:  # Optional: Chinese translation of the description. Leave blank if you cannot provide it.
```

### What if you are unsure about the content? Submit boldly!

You may be unsure about the content description or the category. It doesn't matter, boldly contribute and submit in the best form you think. AWESOME is not a code repository, so our management is very relaxed. Administrators can merge first and then modify immediately; of course, if the contributed content is debatable, we can also communicate during the PR process. Therefore, don't worry, please submit your favorite library!

Even after merging, you can still raise an ISSUE or Discussion to discuss the content.

## 🤝 Contribution Methods

We recommend the following three contribution methods:

1.  **Submit a PR directly through the GitHub website interface** - Suitable for submitting new libraries or modifying library descriptions.
2.  **Contribute through the standard PR process** - Suitable for more complex modifications, such as re-adjusting the library's category.
3.  **Contribute through Issues** - If you are unsure how to create a pull request.

### Method 1: Submit a PR through the GitHub website interface

This method is ideal for small contributions:

1.  **Login:** Make sure you are logged into your GitHub account.
2.  **Create a new file:**
    *   Click "Add file" -> "Create new file".
    *   If you have not yet forked the repository to your account, you will be prompted to fork.
3.  **Write the library's information file**
    *   The file name will be `cli-[urfave].yml`.
    *   Refer to the YML content format above and fill it in.
4.  **Submit changes:** Submit the new file with a descriptive message.
5.  **Create a Pull Request:**
    *   Go to [https://github.com/edwinjhlee/awesome/pulls](https://github.com/edwinjhlee/awesome/pulls) and click "New pull request".
    *   Select the branch in your forked repository that contains your changes.
    *   Add a clear title and description to your pull request.

Maintainers will review your pull request and provide feedback if necessary, and merge it if it meets the standards.

### Method 2: Contribute through the standard PR process

This method is more suitable for larger contributions, such as re-adjusting the library's category, or if you prefer to use a local development environment.

**Step 1: Fork and Clone**

1.  Fork this repository to your GitHub account.
2.  Clone the forked repository to your local computer:

```bash
git clone https://github.com/<your-username>/awesome.git
cd awesome
```

**Step 2: Create a new file and add content**

1.  **File location:** Create a new YAML file in the appropriate category directory in the `lang` directory.
    *   **Example:** For `github.com/urfave/cli` (Go library, category: `cli`), the file path will be `lang/go/cli/cli-[urfave].yml`.
    *   **For codeberg.org:** If the repository is hosted on codeberg.org, include `[codeberg.org]` in the file name: `cli-[urfave][codeberg.org].yml`

2.  **File content:** Use the following YAML format:

    ```yaml
    name: urfave/cli
    repo: github.com/urfave/cli
    desc: A simple, fast, and fun package for building command line apps in Go
    desc-zh:  # Optional: Chinese translation of the description. Leave blank if you cannot provide it.
    ```

**Step 3: Commit and Push Changes**

1.  Add the new file to your Git repository:

    ```bash
    git add lang/go/cli/cli-[urfave].yml
    ```

2.  Commit your changes with a descriptive message:

    ```bash
    git commit -m "Add urfave/cli to awesome-go (cli category)"
    ```

3.  Push your changes to your forked repository:

    ```bash
    git push origin main
    ```

**Step 4: Create a Pull Request**

1.  Go to your forked repository on GitHub.
2.  Click the "Contribute" button, then click "Open pull request".
3.  Make sure the base repository is `edwinjhlee/awesome` and the compare branch is your branch.
4.  Add a clear title and description to your pull request.

**[Optional] Step 5: View the results locally**

If you have [x-cmd](https://x-cmd.com) installed, you can preview the generated README file before submitting a pull request:

```bash
x ws gen go
```

This will generate the `go/README.md` file, allowing you to view your changes.

### Method 3: Contribute through Issues

If you are unsure how to create a pull request, you can suggest a new library by creating an issue.
Although this is the easiest method, it is strongly recommended to contribute through a pull request. Please refer to the steps and demonstrations above.

In addition, if you encounter problems during the PR process, you can join the x-cmd user group for assistance.

- **Wechat**

![wechat](./assets/wechat.png)

- ![telegram](./assets/telegram.png) **[Telegram](https://t.me/x_cmd)**

**Initiate Issue Steps**

1.  Create a new issue [here](https://github.com/edwinjhlee/awsome/issues) and select the "[new library]" template.
2.  Fill out the form containing the repository name and a brief description.



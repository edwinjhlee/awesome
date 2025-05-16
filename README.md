# Awesome Lists

## Language Awesome Lists

| Language                              | README                                                        | Total  |
| :------------------------------------ | :------------------------------------------------------------ | :----- |
| [Python](https://a.x-cmd.com/python)  | [README](https://github.com/edwinjhlee/awesome/lang/python)   | 100    |
| [Deno](https://a.x-cmd.com/deno)      | [README](https://github.com/edwinjhlee/awesome/lang/deno)     | 100    |
| [Node](https://a.x-cmd.com/node)      | [README](https://github.com/edwinjhlee/awesome/lang/node)     | 100    |
| [Bun](https://a.x-cmd.com/bun)        | [README](https://github.com/edwinjhlee/awesome/lang/bun)      | 100    |
| [Java](https://a.x-cmd.com/java)      | [README](https://github.com/edwinjhlee/awesome/lang/java)     | 100    |
| [Kotlin](https://a.x-cmd.com/kotlin)  | [README](https://github.com/edwinjhlee/awesome/lang/kotlin)   | 100    |

## Contributing

There are three ways to contribute to this awesome list:

1.  **Using the GitHub Website (Easy)**
2.  **Using Pull Requests (Recommended)**
3.  **Using Issues (Simplest)**

### 1. Contributing via the GitHub Website

This method is suitable for small contributions and doesn't require any local setup.

1.  **Login:** Ensure you are logged into your GitHub account.
2.  **Create a New File:**
    *   Click "Add file" -> "Create new file".  You will be prompted to fork the repository to your account if you haven't already.
3.  **File Naming:**
    *   The file path should follow the pattern: `[category]-[repo_owner].yml`.
    *   **Example:** For `github.com/urfave/cli` categorized as `cli`, the file name would be `cli-[urfave].yml`.
4.  **File Content:**
    *   Use the following YAML format:

    ```yaml
    name: urfave/cli
    repo: github.com/urfave/cli
    desc: A simple, fast, and fun package for building command line apps in Go
    desc-zh:  # Optional: Chinese translation of the description.  Leave blank if you can't provide one.
    ```
5.  **Commit Changes:** Commit the new file with a descriptive message.
6.  **Create a Pull Request:**
    *   Go to [https://github.com/edwinjhlee/awesome/pulls](https://github.com/edwinjhlee/awesome/pulls) and click "New pull request".
    *   Select the branch in your forked repository containing your changes.
    *   Add a clear title and description to your pull request.

The maintainers will review your pull request, provide feedback if necessary, and merge it if it meets the criteria.

### 2. Contributing via Pull Requests (Recommended)

This method is more suitable for larger contributions or if you prefer working with a local development environment.

**Step 1: Fork and Clone**

1.  Fork this repository to your GitHub account.
2.  Clone the forked repository to your local machine:

    ```bash
    git clone https://github.com/<your-username>/awesome.git
    cd awesome
    ```

**Step 2: Create a New File and Add Content**

1.  **File Location:** Create a new YAML file in the appropriate category directory within the `lang` directory.
    *   **Example:** For `github.com/urfave/cli` (Go library, category: `cli`), the file path would be `lang/go/cli/cli-[urfave].yml`.
    *   **For codeberg.org:** If the repository is hosted on codeberg.org, include `[codeberg.org]` in the filename: `cli-[urfave][codeberg.org].yml`

2.  **File Content:** Use the following YAML format:

    ```yaml
    name: urfave/cli
    repo: github.com/urfave/cli
    desc: A simple, fast, and fun package for building command line apps in Go
    desc-zh:  # Optional: Chinese translation of the description.  Leave blank if you can't provide one.
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
2.  Click the "Contribute" button and then "Open pull request".
3.  Ensure the base repository is `edwinjhlee/awesome` and the compare branch is your branch.
4.  Add a clear title and description to your pull request.

**[Optional] Step 5: Review the Result Locally**

If you have [x-cmd](https://x-cmd.com) installed, you can preview the generated README file before submitting the pull request:

```bash
x ws gen go
```

This will generate the `go/README.md` file, allowing you to review your changes.

### 3. Contributing via Issues (Simplest)

If you're unsure about creating pull requests, you can suggest new libraries by creating an issue.

1.  Create a new issue [here](https://github.com/edwinjhlee/awsome/issues) and choose the "[new library]" template.
2.  Fill out the form with the repository name and a brief description.

While this is the easiest method, contributing via pull requests is highly encouraged.

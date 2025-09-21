# Step-by-Step Workflow (Revised for zen-tasker & gemini-cli)

## 1. Sync and Branch

Start from your main development branch, make sure it’s up to date, then create a new feature branch.

```bash
git checkout dev
git pull origin dev
git checkout -b <feature-branch-name>
# e.g., git checkout -b 003-edit-task-flow
```

## 2. Specify the Feature with gemini-cli

Let the AI know what you want to build.

```bash
gemini specify
```

Example prompt:
```
Allow editing of tasks with double-click. Save edits on Enter or blur.
```

## 3. Create a Technical Plan

Ask gemini-cli to break down the steps.

```bash
gemini plan
```

Example prompt:
```
Create a technical plan to support task editing in the Zen Tasker app.
```

## 4. Generate Implementation Tasks

Get gemini-cli to generate granular tasks.

```bash
gemini tasks
```

Example prompt:
```
List all actionable steps to add task editing, based on the plan.
```

## 5. Implement the Feature

Have gemini-cli generate the code.

```bash
gemini implement
```

Example prompt:
```
Implement the task editing feature as described in the plan and tasks.
```

## 6. Review, Test, and Commit

Check the changes locally and test as needed. Then commit:

```bash
git add .
git commit -m "feat: <short description of the feature>"
# e.g., git commit -m "feat: add task editing"
```

## 7. Push Your Branch

Push the feature branch to GitHub:

```bash
git push origin <feature-branch-name>
```

## 8. Make Pull Requests

- Open a PR from your feature branch to `dev` (or `main`, as appropriate).
- Review and merge via the GitHub web interface.
- Example: merge 003-edit-task-flow → dev, then dev → main/master as needed.

## 9. CI/CD and Final Merge

- Let GitHub Actions run to verify builds and tests.
- After merging to `dev`, repeat the process to merge `dev` into `main/master` (if needed).

---

**Notes:**
- Feature branches are typically named with incremental numbers or descriptive names (e.g., `002-add-the-ability`).
- Merges usually go feature → dev → main/master.
- Always review PRs on GitHub before merging.
- Use gemini-cli for specs, plans, tasks, and code, but do PRs and merges via GitHub.

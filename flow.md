# Step-by-Step Workflow

## Step 1: Prepare the Git Environment

First, make sure your local dev branch is up-to-date and create a new feature branch from it.

### Repo url: https://github.com/rhodge-hash/zen-tasker/tree/dev

```Bash
git checkout dev
git pull origin dev
git checkout -b feature/edit-task
```

## Step 2: Specify the Feature
Tell the AI agent what you're building.

```Bash
/specify
```

Example User Input:
```
Add the ability for a user to edit an existing task. The user should be able to double-click on a task's text to make it editable, press "Enter" or click outside the input field to save the changes.
```

## Step 3: Create the Plan
Use the AI agent to create a technical plan.

```Bash
/plan
```

Example User Input:

```
Create a technical plan to add an edit feature to the Zen Tasker app. The plan should outline the necessary JavaScript changes to handle a double-click event on a list item's text, replace the text with an input field, and save the new value upon completion.
```

## Step 4: Generate the Tasks

Have the AI agent break down the plan into specific tasks.

```Bash
/tasks
```

Input:
```
Generate a list of actionable tasks to implement the task editing feature based on the technical plan.
```

## Step 5: Implement the Code
Have the AI agent write the code for the feature.

```Bash
/implement
```

Example User Input:

```
Implement the code to add the task editing functionality to the Zen Tasker app, following the specified tasks.
```

## Step 6: Push the Code and Create a Pull Request
After the AI agent has finished, you will have a new file with the implemented changes. Now you need to push these changes to GitHub and create a pull request.

```Bash
git add .
git commit -m "feat: add ability to edit tasks"
git push origin feature/edit-task
```

Once the push is complete, go to your GitHub repository and you will see an option to create a Pull Request from feature/edit-task to your dev branch. 
When you open the pull request, your CI/CD workflow will automatically run to verify that the tests and builds pass.


# Revise this workflow for gemini-cli usage.

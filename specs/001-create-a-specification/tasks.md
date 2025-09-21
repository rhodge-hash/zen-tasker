# Tasks: Zen Tasker

**Input**: Design documents from `/home/roy/Desktop/Playground/specs/001-create-a-specification/`
**Prerequisites**: plan.md (required)

## Phase 1: Setup
- [X] T001 Create the `index.html` file in the root of the project.

## Phase 2: Implementation
- [X] T002 Add the basic HTML structure to `index.html`, including a `<h1>` for the title, an `<input>` for new tasks, a `<button>` to add tasks, and a `<ul>` to display the tasks.
- [X] T003 Add CSS within a `<style>` tag in the `<head>` of `index.html` to provide a clean, minimalist look. This should include styles for the overall layout, the input field, the button, and the task list. Completed tasks should have a `text-decoration: line-through;` style.
- [X] T004 Add JavaScript within a `<script>` tag at the end of the `<body>` in `index.html`. This script will handle the following:
    - A function to add a new task to the list.
    - An event listener on the "Add" button to call the add task function.
    - An event listener on the input field to allow adding tasks by pressing the "Enter" key.
    - An event listener on the task list (`<ul>`) to handle clicks for marking tasks as complete and for deleting tasks (using event delegation).

## Phase 3: Deployment
- [X] T005 Create a `.github/workflows/deploy.yml` file to automate the deployment of `index.html` to GitHub Pages on every push to the `main` branch.

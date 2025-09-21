# Tasks: Edit Existing Task

**Input**: Design documents from `/home/roy/Desktop/Playground/specs/002-add-the-ability/`
**Prerequisites**: plan.md (required)

## Phase 1: Implementation
- [X] T001 Modify the event listener on the task list (`<ul>`) to handle a `dblclick` event on the `<span>` element that contains the task text. When a double-click occurs, the `<span>` should be replaced with an `<input>` field containing the current task text.
- [X] T002 Add event listeners to the newly created `<input>` field to handle saving the changes. One event listener should listen for the `keypress` event and save the changes when the "Enter" key is pressed. Another event listener should listen for the `blur` event (when the input field loses focus) and save the changes.
- [X] T003 When saving, if the new task text is empty, the task should be removed from the list. Otherwise, the input field should be replaced with a `<span>` containing the new text.

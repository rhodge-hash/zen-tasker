# Quickstart: Edit Existing Task

This document provides instructions for manually testing the edit task functionality.

## Prerequisites

- A task must exist in the task list.

## Testing Steps

1.  **Add a task:**
    -   Enter "Buy milk" into the input field.
    -   Click the "Add" button.
2.  **Enter edit mode:**
    -   Double-click on the text "Buy milk".
    -   **Expected result:** The text is replaced by an input field containing "Buy milk".
3.  **Save by pressing Enter:**
    -   Change the text to "Buy almond milk".
    -   Press the "Enter" key.
    -   **Expected result:** The task text updates to "Buy almond milk" and is no longer editable.
4.  **Enter edit mode again:**
    -   Double-click on the text "Buy almond milk".
5.  **Save by clicking outside:**
    -   Change the text to "Buy soy milk".
    -   Click anywhere outside the input field.
    -   **Expected result:** The task text updates to "Buy soy milk" and is no longer editable.
6.  **Attempt to save an empty task:**
    -   Double-click on the text "Buy soy milk".
    -   Delete all the text in the input field.
    -   Press the "Enter" key.
    -   **Expected result:** The task is removed from the list.

---
layout: page
title: JupyterHub and Notebooks
parent: Lab Procedures
nav_order: 1
math: mathjax3
---

# JupyterHub Student Guide

This page explains how to log in to the course JupyterHub server, retrieve assignments, complete nbgrader notebooks, and submit your work.

## Before you begin

You will be given a JupyterHub username in the format `first_name.last_name.eceXXXX`, where `eceXXXX` is your course number.

- ECE 3210 students will have usernames ending in `ece3210`.
- Use the exact username provided to you.
- If you have trouble with your account or password, contact the instructor.

The course JupyterHub server is hosted at:

```text
https://quick.users.weber.edu
```

## Logging in for the first time

1. Open your browser and go to `https://quick.users.weber.edu`.
2. Enter the username provided by the instructor.
3. The first time you log in, set your password when prompted.
4. After your password is set, log in to enter JupyterLab.

If you forget your password or cannot log in, contact the instructor. Do not create a second account and do not attempt to guess a different username.

<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/jupyter_hub_login.png" alt="JupyterHub login page at quick.users.weber.edu showing the username field and first-time password setup prompt." style="width: 100%;"></div>


## What you will see in JupyterLab

After logging in, you will arrive in **JupyterLab**. The main items you will use are:

- The **file browser** on the left, which shows your files.
- The **Assignments** page under the Nbgrader tab at the top.

<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/assignments_page_first.png" alt="JupyterLab interface showing the file browser on the left and the Nbgrader Assignments tab at the top." style="width: 100%;"></div>

## How to fetch an assignment

When an assignment is released, it will appear in the **Assignments** tab.

1. Open the **Assignments** tab.
2. Find the assignment name in the released assignments list.
3. Click **Fetch**.
4. Wait for the download to finish.
5. Open the assignment notebook from the location JupyterLab creates for it.

<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/fetched_assignment.png" alt="JupyterLab Assignments tab showing a released assignment with the Fetch button highlighted." style="width: 100%;"></div>

Under the *Downloaded Assignments* section, you can see the assignments you have already fetched. You can click click on the assignment name to open the notebook to start working on it.
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/opened_assignment.png" alt="JupyterLab file browser showing a newly fetched assignment notebook in the user's workspace." style="width: 100%;"></div>

If you do not see an assignment that you expect:

- Make sure you are logged in with the correct course username.
- Refresh the browser once.
- Check the **Assignments** tab again.
- If it still does not appear, contact the instructor.

## How to complete an nbgrader notebook

Each lab or homework will usually contain one or more Jupyter notebooks. These notebooks are prepared for autograding, so you must follow the instructions carefully.

### General rules

- Read the notebook from top to bottom before you start coding.
- Save your work frequently.
- Run cells as you work so that you catch errors early.
- Before submitting, restart the kernel and run all cells to make sure the notebook works from a clean state.

### What you should do

- Enter your answers only where the notebook tells you to do so.
- Replace `# YOUR CODE HERE` and `raise NotImplementedError()` only in the cells meant for student work. This is an example below.  Just replace the placeholder code with your answer, and do not change anything else in the notebook structure.
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/your_code_here.png" alt="Example of a student answer cell in an nbgrader notebook, showing the placeholder code that students are expected to replace." style="width: 100%;"></div>

- Sometimes you are asked to write a function rather than fill in variable values.  In that case, fill in the function body, but do not change the function signature. The autograder tests will call your function by name, so if you change the name or parameters, the tests will fail even if your code is correct.
- Write complete, readable Python code.
- Use Markdown cells only when the notebook asks for a written explanation.
- Keep any required output cells so you can verify your results before submitting.

### What you must not do

- Do not rename the notebook unless the instructions explicitly tell you to.
- Do not add extra cells.
- Do not delete existing cells.
- Do not reorder cells.
- Do not change a cell from code to markdown or from markdown to code.
- Do not delete autograder tests or instructor-provided content.

Changing the notebook structure can cause the autograder to fail, even if your math or code is otherwise correct.

> Screenshot placeholder: Example nbgrader notebook showing a student-answer cell with `# YOUR CODE HERE` and a separate locked test cell.

### Running notebook cells

To run a cell, click inside it and press `Shift+Enter`.

Use this workflow while you work:

1. Read the prompt.
2. Write your code or answer in the correct cell.
3. Run that cell.
4. Run any provided test or check cells that come after it.
5. Fix any errors before moving on.

If a notebook stops responding or variables seem incorrect, use **Kernel -> Restart Kernel**, then run the notebook again from the top.

> Screenshot placeholder: Notebook toolbar or menu showing how to run a cell and how to restart the kernel.

### Written answers, math, and plots

Some assignments ask for more than just code.

- If a question asks for an explanation, write clearly and directly.
- If a question asks for a plot, make sure the plot is generated when the notebook is run.  Often times you will need to plot data.  You can drag your data files (e.g. CSV files) into the notebook file browser (on the left side of the screen) and those will be automatically uploaded with your submission at the end.  
-  For analytical results, it often helps to work the problem out on paper first and then translate the final result into Python.

## Saving your work

JupyterLab usually autosaves, but you should still save manually before closing the notebook or submitting.

- Use **File -> Save Notebook** or press `Command+S` for macOS users or `Ctrl+S` for Windows/Unix users.
- Make sure the notebook has finished saving before you close the browser tab.

## How to submit an assignment

When you are finished:

- Save the notebook.  Make sure that your data files are in the same directory as the notebook so that they will be included in the submission.  Notice in the photo below, the data files are in the same directory as the notebook, and they will be included in the submission when the notebook is submitted.  
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/submission.png" alt="JupyterLab menu showing the Save Notebook option." style="width: 100%;"></div>

- Restart the kernel and run all cells one final time. (You can do this from the top menu: **Kernel -> Restart Kernel and Run All Cells**.)
- Confirm there are no errors. You can tell this by looking for red error messages in the notebook. If there are errors, fix them before submitting.  If you are not sure how to fix an error, ask the instructor before the deadline.
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/no_errors.png" alt="JupyterLab menu showing the Restart Kernel and Run All Cells option." style="width: 100%;"></div>

- Return to the **Assignments** tab.
- Find the assignment.
- Click **Submit**. (The blue **Submit** button next to the assignment name.)
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/submit_button.png" alt="JupyterLab Assignments tab showing the Submit button for a completed assignment." style="width: 100%;"></div>

- You can submit as many times as you like before the deadline, but only your final submission will be graded.  
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/multiple_submissions.png" alt="JupyterLab submission confirmation dialog or submitted-status view." style="width: 100%;"></div>

- After the assignment is graded, the instructor will enter your score on Canvas.  You can also see where you lost points by looking at the feedback in the **Assignments** tab.  Click the **Fetch Feedback** button to download a copy of your notebook with autograder feedback.  You can see a **(view feedback)** link next to the assignment name after feedback is available.  
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/feedback.png" alt="JupyterLab Assignments tab showing the Fetch Feedback button and view feedback link." style="width: 100%;"></div>

- Click that link to open the feedback html version of the notebook in your browser.  The feedback will show you which test cases passed and which ones failed, along with any error messages or hints from the autograder.  Use this feedback to understand your mistakes and improve on future assignments.
<div style="text-align: center;"><img src="/assets/images/lab_images/jupyter_hub_images/feedback_html.png" alt="Example of autograder feedback showing which test cases passed and which ones failed." style="width: 100%;"></div>

Do not assume your work was submitted just because you finished the notebook. You must use the **Submit** button in the **Assignments** tab.


## Before you click submit

Use this checklist every time:

- I answered every required question.
- I only edited the cells intended for student responses.
- I did not add, delete, rename, or reorder cells.
- I ran the notebook from top to bottom without errors.
- I saved the notebook.
- I clicked **Submit** in the **Assignments** tab.

## Common problems

### I cannot log in

- Verify that you are using the exact username given to you.
- If this is your first login, make sure you completed the password setup step.
- If the problem continues, contact the instructor.

### I do not see the Assignments tab

- Make sure the left sidebar is visible.
- Reload the page once.
- Log out and log back in.
- If the tab is still missing, contact the instructor.

### I fetched the assignment, but now I cannot find the notebook

Check the file browser in JupyterLab. The fetched files should appear in your workspace. Open the notebook from there and work on that copy.

### The notebook has errors even though I think my answer is right

- Restart the kernel.
- Run all cells from the top.
- Check variable names, array sizes, units, and function definitions carefully.
- Make sure you did not accidentally edit a test cell or notebook metadata by changing the notebook structure.

### I submitted the wrong thing

If you realize you made a mistake, contact the instructor immediately. Do not assume the system will automatically accept a corrected submission unless you have been told that resubmission is allowed.

## Expectations

- Start early enough that you have time to troubleshoot.
- Keep your work organized.
- Ask questions before the deadline if something is unclear.
- Account and password questions should be directed to the instructor.

If you follow the workflow on this page, most submission problems can be avoided.


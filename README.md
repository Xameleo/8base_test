# 8base Quick Start feedback

The Quick Start guide provides basic information to get started with the service, but has certain problems that may confuse some users

These are the problems i noticed:

- Links that suppose to lead to user workspace sections are lead to https://app.8base.com/developer-home/workspaces page 

- Screenshot in section "2.1 Building a Data Model"  is confusing, the wrong checkbox was selected in the screenshot

- "8base init . --functions=resolver:myCustomResolver" command which proposed in guide to init a project are incorrect, project name cannot start with period or be empty.

**************************************
**Bug-1**

Paragraph 2.1: Data Builder link redirects to https://app.8base.com/developer-home/workspaces page

**Steps to reproduce:**

1. Open Quick Start guide, paragraph 2.1: https://docs.8base.com/docs/getting-started/quick-start/#21-building-a-data-model
2. Click on Data Builder link

**Actual result:** link redirects to https://app.8base.com/developer-home/workspaces page

**Expected result:** link leads to workspace data page or there should be no link at all

**Seriousness**: very low

**************************************

**Bug-2**

Paragraph 2.1: Misguiding screenshot at "Add user to Notes" section

**Steps to reproduce:**

1. Open Quick Start guide, paragraph 2.1: https://docs.8base.com/docs/getting-started/quick-start/#21-building-a-data-model
2. Scroll to "Add user to Notes" section

**Actual result:** Screenshot has "Allow multiple Users per Note" checkbox highlighted and 
"Allow miltiple Notes per User" not hightlighted

**Expected result:** Screenshot has "Allow multiple Users per Note" checkbox NOT highlighted and 
"Allow miltiple Notes per User" hightlighted same as description above screenshot

**Seriousness**: secondary



**************************************

**Bug-3**

Paragraph 2.1: API Explorer link redirects to https://app.8base.com/developer-home/workspaces page

**Steps to reproduce:**

1. Open Quick Start guide, paragraph 2.1: https://docs.8base.com/docs/getting-started/quick-start/#21-building-a-data-model
2. Click on API Explorer link

**Actual result:** link redirects to https://app.8base.com/developer-home/workspaces page

**Expected result:** link leads to workspace API explorer page or there should be no link at all

**Seriousness**: very low

**************************************

**Bug-4**

Paragraph 2.3:  Authentication page link redirects to https://app.8base.com/developer-home/workspaces page

**Steps to reproduce:**

1. Open Quick Start guide, paragraph 2.3: https://docs.8base.com/docs/getting-started/quick-start/#21-building-a-data-model
2. Click on Authentication page link

**Actual result:** link redirects to https://app.8base.com/developer-home/workspaces page

**Expected result:** link leads to workspace Authentication page in App Services or there should be no link at all

**Seriousness**: very low

**************************************

**Bug-5**

Paragraph 3.2: "8base init . --functions=resolver:myCustomResolver" command returns an error

**Description**

Paragraph 3.2 suggests Init new 8base project with one function called myCustomResolver using the
"8base init . --functions=resolver:myCustomResolver" command, which is not correct because "8base init" command
requires project name which cannot start with period or be empty. This is most likely a documentation bug which can confuse user

**Steps to reproduce:**

1. Open 8base CLI
2. Move into any directory
3. Try to init new 8base project with one function called myCustomResolver using the
"8base init . --functions=resolver:myCustomResolver" command as described in Paragraph 3.2 of Quick start

**Actual result:** error: Invalid project name: name cannot start with a period.

**Expected result:** As described in Quick start guide, this command should init new 8base project in working directory

**Seriousness**: secondary

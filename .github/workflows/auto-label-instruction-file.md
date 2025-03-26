# Opened/Edited GitHub issue auto-labeling

When an issue has been created or edited, an effort should be made to label the issue. Labels are important in DevDapp because they allow the underlying API to attribute points to the user for completing a task. The goal of auto-labeling is to assign at least 1 valid task label to an issue so the DevDapp backend can assign the appropriate points to the user.

# Steps

1. Checkout GitHub repo rairprotocol/dev-dapp-season1 folders:
	- ".github/workflows/"
		- This folder holds GitHub Action yaml files, as well as secondary definition files for those actions.
    - "Season 1 Tasks/"
    	- This Folder holds subfolders each with a readme.md file describing each task to be completed by a user and can be used to interpret the appropriate label to apply to an open issue. 
    	- There is a section in each readme.md titled "labels" that describes which labels should be applied if the task is deemed valid. If a task has a sponsor, the appropriate sponsor label should be applied, but only if the awarded label applied first.

2. Get issue number for the event which triggered the GitHub Action:
	- Use issue number to make API calls for the specific event/issue.

3. Determine which task the issue is trying to satisfy:
	- Look through the folders in "Season 1 Tasks/" at the markdown files for each task.
	- Check Issue Title and Issue Body for hints at which task is being completed.

4. Validate the task using the Issue Title and Issue Body text:
	- Valid issues must have body text to verify at the very least.
	- Titles are ancillary, but may be helpful if properly written.
	- Use the browser to validate any hyperlinks included in the body.
		- If the link errors, consider it invalid.
	- If there is no body text, or the body text can not be validated, apply a "Unresolved" label.

5. Apply task label:
	- If a task is valid, apply the appropriate label defined in the markdown, cross reference with ".github/workflows/auto-label-goose.json5".

5. (Optional) Apply sponsored label:
	- Some tasks are sponsored. When a sponsored task is detected, apply the appropriate "Sponsored" label.
	- Example: If the task is sponsored by "Duffman", apply "Sponsored - Duffman" label
	- Only apply sponsored label if a task label has been issued first.
	- If sponsor reads "none", it means there is no corresponding sponsor label


Close the Issue:
	- If a new label for the completed task is successfully added, close the issue.

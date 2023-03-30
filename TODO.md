# Current Task: Add Auto-Update Workflow

A workflow with on.issue.closed would:

Load the CSV at https://raw.githubusercontent.com/refined-github/yolo/main/broken-features.csv

Find the current issue/PR in it

If it's found, leave a comment in the current issue:

This issue has been fixed and will appear in the next version. Ensure that the hotfix is disabled there. Add ${npx utc-version --short} to https://github.com/refined-github/yolo/edit/main/broken-features.csv
Note: The "next version" doesn't need to exist, it's just compared to the "current version"

Related: https://www.npmjs.com/package/utc-version

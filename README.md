# Development Branch Notes

## What is Development Branch?
The development branch is where all feature branches merge first. 
It acts as the integration layer before code moves to staging.
Think of it as the team's shared sandbox for combining work.

## Team Workflow 
Every developer creates their feature branch from development.
When the feature is complete, a pull request is raised to merge back.
The team reviews the code before it gets merged in.

## Integration Testing
Once features are merged into development, integration tests run.
These tests check that multiple features work together correctly.
Any failures must be fixed before moving to staging.

## Daily Practice
Developers pull from development every morning before starting work.
This ensures you always have the latest changes from teammates.
It reduces merge conflicts later in the day.

## Code Reviews
No code gets merged into development without a review.
At least one teammate must approve your pull request.
This maintains code quality across the team.

## Environment Variables
Development branch uses its own set of environment variables.
These point to dev databases, not production data.
Never use production credentials in the development branch.

## Branch Naming Convention
Feature branches follow the pattern: feature/feature-name.
Bug fix branches follow: bugfix/issue-description.
Always use lowercase with hyphens, no spaces.

## Merging Rules
Rebase your feature branch on development before raising a PR.
This keeps the commit history clean and linear.
Squash multiple WIP commits into one meaningful commit.

ADDED
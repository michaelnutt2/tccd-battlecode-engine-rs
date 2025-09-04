# Life Cycle of a Pull Request
It’s important to break your feature down into small pieces first. Each piece should become its own pull request. Small, focused pull requests are easier to review and merge.
Once you know what the first small piece of your feature will be, follow this general process while working:
1. [Create a new branch, following our Git Workflow.](docs/GIT.md)
2. Make your first commit. We need at least one commit to create the initial pull request.
3. Open the pull request on GitHub. Prefix the title with a general area, e.g. `feat(engine):` or `fix(world):`. Use [Conventional Commits](https://www.conventionalcommits.org/) as a guideline.
  - Write a detailed description of the problem you are solving, the part of the engine it affects, and how you are solving it.
  - If the PR is still a work-in-progress, please mark it as a draft. This indicates that the pull request isn’t ready for a final review but welcomes early feedback.
4. Continue developing and pushing commits to your branch.
  - Push your changes frequently.
  - Before you ask for a review, make sure your branch is up-to-date with the `main` branch.
5. When your PR is ready for a final review, take these steps:
  - Run the automated checks locally:
    - `cargo fmt` to format the code.
    - `cargo clippy -- -D warnings` to lint the code.
    - `cargo test` to run the test suite.
  - Mark the PR as "[Status] Ready for review" on GitHub.
  - You can use GitHub's features to request reviews from specific contributors if you'd like.
6. A reviewer may request changes. Once you've addressed them, the PR can be approved.
7. Once approved, a maintainer will merge your pull request into the `main` branch. Congratulations!

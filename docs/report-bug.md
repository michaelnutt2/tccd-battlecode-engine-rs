# Creating a Great Bug Report
The [Issues tab](https://github.com/michaelnutt2/tccd-battlecode-engine-rs/issues) is a ticket database used to track projects and bugs. It's designed to make it as simple as possible for people to report bugs and suggest features.
## Three Steps to a Great Bug Report
### 1. Make Sure the Bug is Really a Bug
Before you report a bug, make sure it's not just an issue with your local environment.
- Ensure you are on the latest `main` branch.
- Make sure your Rust toolchain is up to date (`rustup update`)
- Clean your build artifacts (`cargo clean`) and rebuild the project (`cargo build`).
Do you still see the issue? If so, you might have found a bug!
### 2. See if It's Already Been Reported
To check if a bug has already been reported, you can:
- Look through the [current list of Open Issues](https://github.com/michaelnutt2/tccd-battlecode-engine-rs/issues).
- Use the search bar to look for keywords related to your issue.
Not mentioned anywhere? It's time to create a new issue!
### 3. Create a New, Detailed Issue
A detailed bug report helps us fix problems faster. When you create an issue, please include the following:
- **A clear, descriptive title:** e.g., "Engine panics when a robot moves to coordinates (0, -1)".
- Your Environment:
  - Operating System (e.g., Ubuntu 22.04, Windows 11, macOS Sonoma)
  - Rust version (`rustc --version`)
- **Steps to Reproduce:**
  - Provide a clear, step-by-step list of actions to trigger the bug.
  - If possible, include the map file and player code that causes the issue.
- **What You Expected to Happen:** _e.g., "The robot should move to the new location without an error."_
- **What Actually Happened:** _e.g., "The engine panicked with the error message: `thread 'main' panicked at 'attempt to subtract with overflow'`."_
- **Screenshots or Logs:** If there are console logs or other relevant output, please include them.
## Contribute and Comment on Existing Issues
If you find an issue that you are also experiencing, please add a "thumbs up" reaction to it. If you have new information to add, such as a different way to reproduce it, feel free to leave a comment.

# rfSE Sprint Check Details

Welcome to the rfSE Club's Sprint Check.

## Submission Instructions

To contribute your solutions, follow these steps to fork the repository, add your solutions, and submit a pull request:

1. **Fork the Repository**:

   - Go to the repository on GitHub.
   - Click the **Fork** button at the top-right to create a copy of the repository under your GitHub account.

2. **Clone Your Fork**:

   - Clone your forked repository to your local machine using:
     ```
     git clone <your-forked-repo-url>
     ```
   - Navigate to the repository folder:
     ```
     cd <repository-name>
     ```

3. **Switch to the Submissions Branch**:

   - Switch to the `submissions` branch.

   ```
   git switch origin/submissions
   ```

4. **Create a Folder with Your Name**:

   - Inside the repository, create a folder named after yourself (e.g., `John_Doe`).
     ```
     mkdir Your_Name
     ```

5. **Add Your Solutions**:

   - Create a file (e.g., `sprint-1-check-solutions.md` or `sprint-1-check-solutions.txt`) inside your folder.

   - Create a file (e.g., `sprint-1-check-theory-solutions.md` or `sprint-1-check-theory-solutions.txt`) inside your folder.

6. **Commit Your Changes**:

   - Add your folder and solutions file to git:
     ```
     git add .
     ```
   - Commit with a clear message:
     ```
     git commit -m "Add solutions by Your_Name for Sprint 1"
     ```

7. **Push to Your Fork**:

   - Push your changes to the `submissions` branch of your forked repository:
     ```
     git push origin submissions
     ```

8. **Create a Pull Request (PR)**:
   - Go to your forked repository on GitHub.
   - Switch to the `submissions` branch.
   - Click **New Pull Request**.
   - Set the base repository to the original repo’s `submissions` branch and your fork’s `submissions` branch as the compare branch.
   - Add a title (e.g., "Sprint 1 Solutions by Your_Name") and a brief description.
   - Click **Create Pull Request**.

## Guidelines

- Ensure your folder is named exactly as your name (e.g., `First_Last`) to avoid conflicts.
- Submit solutions in a clear, organized format (preferably Markdown or plain text).
- Only submit to the `submissions` branch; PRs to other branches will be rejected.
- Double-check your time and space complexity calculations for accuracy.
- Submit by the deadline communicated by the rfSE club.

## Need Help?

- If you're new to Git/GitHub, refer to [GitHub's PR guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
- Reach out to the rfSE Club club’s slack channel for assistance.

Happy coding!

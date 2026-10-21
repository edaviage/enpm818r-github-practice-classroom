# Commit Before the VM Times Out

This short exercise is practice for saving your work before an ephemeral AWS practice VM shuts down. The VM is available for 20 minutes. Your work must be committed and pushed to GitHub before then.

## What to do

1. Fork this repository to your own GitHub account.
2. On the practice VM, clone your fork:

   ```bash
   git clone https://github.com/YOUR-GITHUB-USERNAME/enpm818r-github-practice-classroom.git
   cd enpm818r-github-practice-classroom
   ```

3. Create a branch named `practice/<your-umd-id>` using your UMD directory ID in lowercase:

   ```bash
   git switch -c practice/your-umd-id
   ```

4. Append one line to `practice-log.md` containing your UMD ID and the current UTC date and time. For example:

   ```text
   - UMD ID: abcd1234 — committed at 2026-10-21 14:05 UTC
   ```

   Use your UMD ID, not your full name. This repository is public.

5. Commit and push your branch to your fork:

   ```bash
   git add practice-log.md
   git commit -m "Add my practice checkpoint"
   git push -u origin practice/your-umd-id
   ```

6. Open a PR from your fork to the course repository's `main` branch. Set the title to exactly:

   ```text
   Practice submission: your-umd-id
   ```

An open PR or a merged PR counts as a completed submission. A closed, unmerged PR does not. Keep your commit and push steps ahead of the VM timeout; work that exists only on the VM will be lost.

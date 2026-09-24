# 💸 The Ultimatum Game: GitHub PR Edition

In this assignment, you will practice creating branches, opening Pull Requests (PRs), configuring repository permissions, and responding to automated code reviews using GitHub Actions.

---

## 🎯 Objectives

- Practice git branching, committing, and opening Pull Requests.
- Configure repository **Workflow Permissions** and enable **GitHub Actions**.
- Interact with an automated code review bot.
- Experience a classic behavioral economics experiment.

---

## 🧪 The Scenario

You and your partner (an automated GitHub Bot) have been given **$100**.  
You must propose how to divide the money by writing an offer in your repository.

> **Offer Format:** `I offer $X to my partner.` *(Replace `X` with any integer from 0 to 100)*

The bot will automatically evaluate your PR:
- ✅ **Accept ($30 or more):** The offer is fair. You both split the money accordingly.
- ❌ **Reject (Less than $30):** The offer is too low. Neither of you gets anything.

---

## ⚙️ Step 1: Fork & Required Configuration

Before creating your offers, you **must** configure your repository permissions so the automation bot can run.

1. **Fork this repository** to your personal GitHub account.
2. **Enable GitHub Actions:**
   - Click the **Actions** tab at the top of your forked repository.
   - Click the green button: **"I understand my workflows, go ahead and enable them."**
3. **Set Workflow Read/Write Permissions:**
   - Go to your repository **Settings** → **Actions** → **General**.
   - Scroll down to **Workflow permissions**.
   - Select **Read and write permissions**.
   - Click **Save**.

---

## 🛠️ Step 2: Assignment Workflow

You are required to create **at least 3 separate branches** and **3 subsequent Pull Requests**. 

> ⚠️ **CRITICAL WARNING:** Always open PRs against **YOUR OWN FORK** (`your-username/main`). **DO NOT** open Pull Requests against the original upstream repository.

### Requirements Breakdown
* **Total PRs:** Minimum of 3 complete pipeline runs.
* **Outcome Mix:** Must contain at least **1 Accepted PR** ($\ge \$30$) and at least **1 Rejected PR** ($<\$30$).

### Procedure for Each PR (Repeat at least 3 times):

1. **Create a new branch** in your fork (e.g., `offer-1-reject`, `offer-2-accept`, `offer-3`).
2. **Create a file** named `offer.txt` in the root directory of your repository.
3. **Add your offer sentence**:
   ```text
   I offer $X to my partner.
   ```
4. **Commit and push** your branch to your GitHub fork.
5. **Open a Pull Request** comparing your branch against your fork's `main` branch (`your-username:main`).
6. **Wait for the Offer Bot** to run its checks and leave a review comment.
7. **Leave a Comment:** Based on the bot's review, write a comment on your own PR stating either `"Accept"` or `"Reject"`.
8. **Finalize the PR:**
   - If **Accepted** ✅: Merge the PR into your `main` branch.
   - If **Rejected** ❌: Close the PR without merging.

---

## 💡 Tips & Troubleshooting

- **Bot Not Responding?** Ensure you completed Step 1 (enabled Actions tab **AND** set Workflow Permissions to *Read and Write*).
- **Branch Strategy:** Make sure to switch back to `main` before creating each new feature branch to keep your history clean.
- **Fairness:** Consider behavioral economics—what threshold makes an offer rational vs. emotionally acceptable?

---

## 💾 Submission Requirements

Submit a document containing the following:

1. **Link to your GitHub Fork** *(If your fork is set to private, ensure you grant view access to your instructor)*.
2. **Screenshots of your 3+ workflow pipelines** from the **Actions** tab showing successful execution runs.

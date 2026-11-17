# Papermark Upstream Copy & Licensing Notes

## 1. Repository & Upstream Setup
- *My Fork URL:* https://github.com/Sharjilzaidi29/papermark
- *Upstream URL:* https://github.com/papermark/papermark
- *Starting Upstream Commit:* ed10717 (fix(groups): keep existing domains when adding another)

## 2. How Upstream Changes Are Synced
bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main

*(Verified by running `git fetch upstream` and git merge upstream/main in the repository).

## 3. Secrets & Security Check
- Checked tracked files using git ls-files.
- Verified that no .env files, real API keys, or credentials are committed in the repository (only .env.example template exists).

## 4. Short Licensing Note (For Mentor Review)
- **Core Application License:* Papermark core codebase is licensed under *AGPL-3.0 (GNU Affero General Public License v3.0).
- **Enterprise Edition (ee/) & Commercial Terms:* Features under ee/ (Enterprise Edition) are governed by commercial/source-available terms and require a commercial license from Papermark for proprietary/enterprise use.
- *What AGPL-3.0 Allows & Requires When Running for Other People:
  - **Allowed:* You can freely run, modify, and self-host the open-source core version for yourself or for other users over a network.
  - *Required / Must Confirm First:* Because AGPL-3.0 has a strong network copyleft clause, if you modify the code and run it as a hosted service for other people over a network, you *must make the complete corresponding source code of your modified version available* to those users under AGPL-3.0. Also, you must not enable or redistribute proprietary ee/ features without a valid commercial agreement.

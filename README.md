# Pocket AI — initial source build

Native iPhone chat, adapted from Apple's MLX Swift chat sample at commit 378f2449c257788c5067b9f8b086731d76b39b33.
Original license and attribution are retained. Qwen3 0.6B 4-bit is the default;
1.7B is an optional larger model. Model weights download separately on first use.

## Build
Upload this folder to your GitHub repository including the .github folder.
Run Actions → Build Pocket AI for iPhone → Run workflow.
Download the Pocket-AI-unsigned artifact when the build succeeds.
The IPA is UNSIGNED and is not installable until signed for your iPhone.
Enter Apple credentials only in your chosen local signing tool, never in this repo.
Free personal-team signing normally needs renewal after seven days.

## Verify on the phone
Download the small model over Wi-Fi and send a test message. Then force-close the
app, enable Airplane Mode, relaunch and send another message. Offline cold-start
and cache retention are NOT yet verified. Do not delete the app when refreshing:
that may delete its model data. No PC chat server is used by the app.

## Current validation
Source edits and workflow packaging checked on Windows. Compilation, model
download, inference, signing and Airplane Mode require the Mac build/iPhone test.
Do not treat this initial source package as a tested installed app.

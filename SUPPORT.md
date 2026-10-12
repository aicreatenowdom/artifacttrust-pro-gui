# ArtifactTrust Pro GUI support

Contact **AI Creations Now Software Development** at [info@aicreatenow.com](mailto:info@aicreatenow.com) or **1-866-315-4750**.

[Official website](https://trustprogui.com/) · [Setup & Help](https://trustprogui.com/help.html) · [Download version 3.1](https://trustprogui.com/download.html) · [Company website](https://aicreatenow.com/)

## Tell us what happened

Include:

- Your application version and Windows version.
- The stage that failed: installation, first-launch prerequisite preparation, Microsoft sign-in, resource selection, signing, verification, or PDF reporting.
- The exact error message and what you were doing immediately before it appeared.
- Whether you selected one file or a batch, and the affected file types.
- Whether the file was signed successfully even if its PDF report could not be created.

Remove passwords, authentication codes, tokens, private file contents, and other sensitive information from screenshots and logs. Send private account matters by email instead of posting them in a public GitHub issue. Do not send a file that you are not authorized to share.

## Quick checks

**Preparation:** Required Microsoft packages are bundled. Their preparation takes place after the first application launch and acceptance of the installation agreement, not during Setup. Administrator access is required. Tell us which component or readiness check reported an error.

**Microsoft resources:** Confirm that you have an eligible identity, Azure subscription, configured Microsoft Artifact Signing account, active Public Trust certificate profile, and signing permissions. This workflow supports the standard Azure public cloud. Microsoft manages account eligibility, identity validation, certificate profiles, service restrictions, and billing.

**File selection:** Select compatible unsigned Windows files smaller than 4 GB each. Confirm write access and enough space for original backups. Existing signed files and the running application itself are rejected by this workflow.

**PDF reports:** A three-page report is generated for single-file signing only. Batches of 2–50 files have per-file results without PDF reports. Report generation can fail independently of signing; check the actual signature result before assuming the file is unsigned.

**Saved sign-in:** Closing the app keeps its own authorization cache. Use **Sign out of this program** or uninstall to remove product-owned authorization. These operations do not sign out unrelated Microsoft or browser sessions. Microsoft may require reauthentication at any time.

**Security warnings:** Code signing does not guarantee acceptance by SmartScreen, antivirus vendors, Microsoft Store, or other platforms. Provide the exact warning and the version of the software displaying it.

## Downloads, policies, and repository contents

ArtifactTrust Pro GUI is free for everyone; optional donations are not required for use. Microsoft service costs are separate. ArtifactTrust Pro GUI is [available on Microsoft Store](https://apps.microsoft.com/detail/xp8lcmjczs31dn?hl=en-US&gl=US). You can also use the [official direct download](https://download.aicreatenow.com/software/ArtifactTrustPro3.1.0microsoft.exe) for the current Windows installer.

GitHub's **Code → Download ZIP** contains this repository's product documentation and artwork, not the application or its source code.

[Getting started](GETTING-STARTED.md) · [Product overview](README.md) · [Privacy & Installation Agreement](https://trustprogui.com/privacy.html) · [Terms & Donations](https://trustprogui.com/terms.html)

# Getting started with ArtifactTrust Pro GUI

**Version 3.1 · Windows x64 · Free for everyone**

[Download the installer](https://download.aicreatenow.com/software/ArtifactTrustPro3.1.0microsoft.exe) · [Official website](https://trustprogui.com/) · [Video walkthrough](https://download.aicreatenow.com/media/aicreatenow/artifacttrust.mp4)

## Before your first signature

You need Windows 10 version 1809 or later, or Windows 11, on a 64-bit x64 PC, administrator access, and an internet connection. You also need your own eligible Microsoft identity, Azure subscription, configured Microsoft Artifact Signing account, active **Public Trust** certificate profile, and permission to sign.

The application supports the standard Azure public cloud. Private Trust profiles and sovereign-cloud endpoints are not supported by this workflow. Microsoft account setup, identity validation, service eligibility, and charges are separate from this free application.

## Install, connect, and sign

1. **Install the application.** Run `ArtifactTrustPro3.1.0microsoft.exe` and follow the installer. The default folder is `C:\Program Files\ArtifactTrust Pro GUI`; you can choose another dedicated folder.
2. **Launch the desktop shortcut.** Review the Privacy and Installation Agreement. After consent, System Readiness prepares missing Microsoft components from the bundled packages and reuses suitable existing installations. Setup itself does not prepare prerequisites or launch the application.
3. **Connect your signing resources.** Sign in through Microsoft, then select your subscription, signing account, and active Public Trust certificate profile. Complete any Microsoft authentication or MFA prompts.
4. **Select the files.** Choose one compatible unsigned Windows file or a batch of 2–50 files. Each must be smaller than 4 GB and accessible for writing. The application creates and verifies an unsigned backup alongside each selected file before signing.
5. **Sign and review.** Signing modifies the selected file in place. The application checks the resulting signature and timestamp. Keep your original release backups and review the actual results before distribution.

![ArtifactTrust Pro GUI 3.1 file review screen](assets/artifacttrust/review-files.webp)

## Choose the right workflow

| Workflow | Files | What to review |
|---|---:|---|
| Single-file signing | 1 | Signed file, signature and timestamp verification, and a three-page PDF report |
| Batch signing | 2–50 | Files processed sequentially with one profile; per-file results; no PDF reports |

The PDF report records information about the signed software file. It is not a PDF document-signing feature. Open or print reports using your Windows PDF viewer.

## Common questions

**Is the app free?** Yes. No application purchase or donation is required. Microsoft subscriptions and signing-service charges remain separate. [Optional coffee donations](https://buy.stripe.com/6oUeVf77ZdRCfMEbka5kk04) support development without unlocking features.

**What is bundled?** Azure CLI and its Artifact Signing extension, .NET 8 x64 Runtime, Microsoft Visual C++ x64 Redistributable, Windows SDK Signing Tools, and Microsoft Artifact Signing Client Tools. The app also includes its own self-contained .NET runtime. Preparation uses bundled packages; authentication, signing, timestamping, and certificate checks still need network access.

**Which files can I sign?** Compatible unsigned Windows software files, including EXE, DLL, and MSI, smaller than 4 GB each. A file appearing in the picker does not guarantee it meets every package or driver signing requirement. Existing signatures are not overwritten, and the running application cannot sign itself.

**Where are files and reports handled?** Selected files, original backups, hashes, and reports are handled locally. The application uses Microsoft's signing client and services for authentication and signing. It does not upload your selected files to AI Creations Now. See the [Privacy and Installation Agreement](https://trustprogui.com/privacy.html) for the full data and component disclosures.

**Why did signing succeed but the PDF fail?** Report generation is a separate step. A PDF error does not automatically mean the file's signature failed. Review the result and the file's signature, and check storage and write permissions before requesting support.

**Will I need to sign in every time?** The app retains its own local authorization for convenient repeat use. Microsoft and your organization control session policies and may require authentication again. There is no guaranteed sign-in duration.

**How do I sign out?** Select **Sign out of this program** to remove the application's saved authorization. Closing the application keeps the saved session. The sign-out control does not clear unrelated browser, Windows, Office, or ordinary Azure CLI sessions.

**What does uninstall remove?** Successful uninstall removes the application's dedicated folder, shortcuts, uninstall entry, and product-owned authentication caches. Shared Microsoft prerequisites remain installed. Signed files, backups, and reports outside the application folder are preserved. Use a dedicated install folder and keep unrelated files elsewhere.

**Will signing eliminate security warnings?** No. A signature identifies the publisher on the certificate and helps detect changes. Windows, Microsoft Store, antivirus vendors, and other platforms apply their own acceptance and reputation policies.

**Is it in Microsoft Store?** Submission is awaiting approval. The free direct installer is available now.

## Silent deployment

```text
ArtifactTrustPro3.1.0microsoft.exe /VERYSILENT /SUPPRESSMSGBOXES /SP- /NORESTART /RESTARTEXITCODE=3010
```

These switches control Setup and prevent a forced Setup restart. They do not launch the application, prepare prerequisites, bypass first-use consent, or automate Microsoft authentication. Launch the installed shortcut when ready to complete those steps.

## More information

[Full setup guide](https://trustprogui.com/help.html) · [Application screenshots](https://trustprogui.com/screenshots.html) · [Privacy & Installation Agreement](https://trustprogui.com/privacy.html) · [Third-Party Notices](https://trustprogui.com/legal/THIRD-PARTY-NOTICES.txt)

[Back to product overview](README.md) · [Contact support](SUPPORT.md)

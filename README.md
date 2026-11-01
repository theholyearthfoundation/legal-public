<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/theholyearthfoundation/.github/main/profile/assets/banner-dark.svg">
  <img alt="The Holy Earth Foundation: the foundation's golden heart within a breathing halo, framed by a living vine. The banner moves gently; with reduced motion it shows still." src="https://raw.githubusercontent.com/theholyearthfoundation/.github/main/profile/assets/banner-light.svg" width="100%">
</picture>

<img src="assets/icons/scale.svg" width="56" height="56" alt="">

# The Holy Earth Foundation: legal, the public lane

![Lane](https://img.shields.io/badge/Lane-public_witness-d97706?style=flat-square)
![Carries](https://img.shields.io/badge/Carries-folder_map_and_policy_skeletons-6b4f1d?style=flat-square)
![Edits](https://img.shields.io/badge/Edits-by_sync_only-b45309?style=flat-square)
![For](https://img.shields.io/badge/For-Visitors-64748b?style=flat-square)

*How The Holy Earth Foundation keeps its paperwork, shown in the open: the folder map and the skeletons of the
policies it is writing. The paperwork itself stays private.*

</div>

## <img src="assets/icons/compass.svg" width="24" height="24" alt=""> What this is

The foundation keeps its legal paperwork in one **private** repository, `theholyearthfoundation/legal` (officers and
counsel only; a visitor who opens that link sees a 404). This public repository is its **witness**: a workflow copies
into it only the policy skeletons and their icons, after a check that reads every file, and nobody edits it by hand.

## <img src="assets/icons/folder-lock.svg" width="24" height="24" alt=""> The folder map (private side)

| | Folder | What it holds | Here? |
|---|---|---|---|
| <img src="assets/icons/landmark.svg" width="16" height="16" alt=""> | `entity/` | formation papers, bylaws, state registrations, the officer roster | never |
| <img src="assets/icons/file-text.svg" width="16" height="16" alt=""> | `tax/` | returns and their working papers, by year | never |
| <img src="assets/icons/files.svg" width="16" height="16" alt=""> | `filings/` | what is sent to or received from a government that is not a tax return | never |
| <img src="assets/icons/message-circle-question.svg" width="16" height="16" alt=""> | `counsel/` | questions for a CPA or an attorney, and their answers | never |
| <img src="assets/icons/scroll-text.svg" width="16" height="16" alt=""> | `policies/` | the policies the foundation holds itself to | only [`policies/skeletons/`](policies/skeletons/) |

```mermaid
flowchart LR
  subgraph PRIVATE["theholyearthfoundation/legal (private)"]
    E["entity/ tax/<br/>filings/ counsel/"]
    S["policies/skeletons/"]
    A["policies/ (adopted)<br/>policies/signed/"]
  end
  S -->|"allowlist + two tripwires<br/>(every file read)"| PUB["theholyearthfoundation/legal-public<br/>(this repository)"]
  E -. "refused by path,<br/>whatever any list says" .-x PUB
  A -. "not listed" .-x PUB
```

## <img src="assets/icons/scroll-text.svg" width="24" height="24" alt=""> The policy skeletons

Headings and plain questions for the foundation's officers and counsel. **None is an adopted policy, and none states a
fact about The Holy Earth Foundation.** *Not legal advice.*

| | Skeleton |
|---|---|
| <img src="assets/icons/users.svg" width="16" height="16" alt=""> | [Conflict of interest](policies/skeletons/conflict-of-interest.md) |
| <img src="assets/icons/hand-heart.svg" width="16" height="16" alt=""> | [Gift acceptance](policies/skeletons/gift-acceptance.md) |
| <img src="assets/icons/landmark.svg" width="16" height="16" alt=""> | [Treasury and digital assets](policies/skeletons/treasury-and-digital-assets.md) |
| <img src="assets/icons/history.svg" width="16" height="16" alt=""> | [Document retention](policies/skeletons/document-retention.md) |

## <img src="assets/icons/shield-alert.svg" width="24" height="24" alt=""> Please do not edit this repository by hand

Everything except this README is copied in by a workflow in the private repository, and the next copy replaces hand
edits. The rule it follows: *a public lane never publishes a file a machine or a person has not read.* The procedure is
SOP-OPS-003 in the foundation's procedures ([public twin](https://github.com/theholyearthfoundation/ops-standard-operating-procedures-public)).

<sub>The Holy Earth Foundation · [theholyearthfoundation.github.io](https://theholyearthfoundation.github.io) · [on GitHub](https://github.com/theholyearthfoundation) · Icons: Lucide (ISC) · Prepared 2026-11-01.</sub>

# Local branch & PR health report

- **Generated:** 2026-06-24 06:18 UTC
- **Repo:** zed-industries/zed (origin) / OmChillure/zed (fork)
- **origin/main:** `daf4656c871f`
- **Current branch:** `mouse-bindings-v2`
- **Local branches audited:** 66
- **Author PRs (all states):** 63 (OPEN=5, MERGED=32, CLOSED=26)

## Executive summary

| Verdict | Count |
|---------|------:|
| KEEP (active / open PR / main) | 6 |
| KEEP_REVIEW (unique / closed-unmerged) | 23 |
| DELETE_SAFE (merged / duplicate / on main) | 37 |

### Open PRs on zed-industries/zed (yours)

- **#55490** [Support loading Git commit templates when remote](https://github.com/zed-industries/zed/pull/55490) — branch `fix-git-tempalte-do-not-work-in-reote` — labels: area:integrations/git — +45/−2 — updated 2026-05-03
- **#55216** [Add user-configurable mouse and scroll wheel keybindings](https://github.com/zed-industries/zed/pull/55216) — branch `mouse-bindings-v2` — labels: — — +546/−21 — updated 2026-06-23
- **#54907** [svg_preview: Add zoom and pan support](https://github.com/zed-industries/zed/pull/54907) — branch `fix-zoom-pan-not-possible-in-svg-preview` — labels: — — +537/−25 — updated 2026-04-26
- **#52849** [Fix MCP servers in multi root workspaces](https://github.com/zed-industries/zed/pull/52849) — branch `fix-mcp-servers-in-multi-root-wrokspaces` — labels: — — +193/−7 — updated 2026-03-31
- **#52671** [Fix tab switcher random jumps](https://github.com/zed-industries/zed/pull/52671) — branch `fix-tab-switcher-random-jumps` — labels: — — +89/−2 — updated 2026-05-05

## Open PRs categorized by area

### gpui / input

- #55216 `mouse-bindings-v2` — Add user-configurable mouse and scroll wheel keybindings

### integrations/git

- #55490 `fix-git-tempalte-do-not-work-in-reote` — Support loading Git commit templates when remote

### project / MCP

- #52849 `fix-mcp-servers-in-multi-root-wrokspaces` — Fix MCP servers in multi root workspaces

### svg_preview

- #54907 `fix-zoom-pan-not-possible-in-svg-preview` — svg_preview: Add zoom and pan support

### tab_switcher

- #52671 `fix-tab-switcher-random-jumps` — Fix tab switcher random jumps

## Conflict risk vs `mouse-bindings-v2` (PR #55216)

Touched files on #55216:
- `crates/editor/src/actions.rs`
- `crates/editor/src/element.rs`
- `crates/editor/src/navigation.rs`
- `crates/gpui/src/key_dispatch.rs`
- `crates/gpui/src/platform/keystroke.rs`
- `crates/gpui/src/window.rs`

### Your other open PRs — overlap rank

| Rank | PR | Branch | Overlapping files | Keymap touch | Score | Risk |
|-----:|----|--------|-------------------|:------------:|------:|------|
| 1 | #55490 | `fix-git-tempalte-do-not-work-in-reote` | — | no | 0 | LOW |
| 2 | #54907 | `fix-zoom-pan-not-possible-in-svg-preview` | — | **yes** (default-*.json) | 3 | MEDIUM |
| 3 | #52849 | `fix-mcp-servers-in-multi-root-wrokspaces` | — | no | 0 | LOW |
| 4 | #52671 | `fix-tab-switcher-random-jumps` | — | no | 0 | LOW |

Notes:
- **#54907** (svg zoom/pan) edits default keymaps only — low direct conflict with gpui mouse binding plumbing, but both change input/keymap surface area.
- **#55490, #52849, #52671** touch unrelated crates — negligible conflict risk with #55216.

### Local branches with file overlap on #55216 paths (incl. superseded)

| Score | Branch | Overlap | PR state | Verdict |
|------:|--------|---------|----------|---------|
| 60 | `backup/mouse-bindings-v2-before-rewrite` | `crates/editor/src/actions.rs`, `crates/editor/src/element.rs`, `crates/editor/src/navigation.rs`, `crates/gpui/src/key_dispatch.rs`, `crates/gpui/src/platform/keystroke.rs`, `crates/gpui/src/window.rs` | — | DELETE_SAFE |
| 60 | `scratch/mouse-bindings-backup` | `crates/editor/src/actions.rs`, `crates/editor/src/element.rs`, `crates/editor/src/navigation.rs`, `crates/gpui/src/key_dispatch.rs`, `crates/gpui/src/platform/keystroke.rs`, `crates/gpui/src/window.rs` | — | DELETE_SAFE |
| 40 | `user-configurable-mouse-bindings` | `crates/editor/src/actions.rs`, `crates/editor/src/element.rs`, `crates/gpui/src/key_dispatch.rs`, `crates/gpui/src/window.rs` | CLOSED | DELETE_SAFE |
| 10 | `clickable-breadcrumbs` | `crates/editor/src/element.rs` | — | KEEP_REVIEW |
| 10 | `fix-breakpoint-placement-guards` | `crates/editor/src/element.rs` | CLOSED | KEEP_REVIEW |
| 10 | `fix-numbering-for-indented-list` | `crates/editor/src/element.rs` | CLOSED | KEEP_REVIEW |
| 10 | `fix-two-focused-states` | `crates/gpui/src/window.rs` | MERGED | DELETE_SAFE |

**Highest conflict candidate among live work:** only `user-configurable-mouse-bindings` (CLOSED #53889) shares the same problem space; it is superseded by `mouse-bindings-v2` and safe to delete locally.

## Full local branch audit

| Branch | Ahead | Behind | Tip on main? | Fork remote | Unpushed | PR | State | Kind | Verdict |
|--------|------:|-------:|:------------:|:-----------:|---------:|----|-------|------|---------|
| `fix-tab-switcher-random-jumps` | 2 | 2145 | no | yes | 0 | #52671 | OPEN | open_pr | **KEEP** |
| `fix-mcp-servers-in-multi-root-wrokspaces` | 5 | 2057 | no | yes | 0 | #52849 | OPEN | open_pr | **KEEP** |
| `fix-zoom-pan-not-possible-in-svg-preview` | 2 | 1271 | no | yes | 0 | #54907 | OPEN | open_pr | **KEEP** |
| `fix-git-tempalte-do-not-work-in-reote` | 1 | 1173 | no | yes | 0 | #55490 | OPEN | open_pr | **KEEP** |
| `main` | 0 | 57 | yes | yes | 0 | — | — | main | **KEEP** |
| `mouse-bindings-v2` * | 2 | 7 | no | yes | 0 | #55216 | OPEN | active_open_pr | **KEEP** |
| `responsive-panel-sizing` | 1 | 3470 | no | no | — | #49224 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-breakpoint-placement-guards` | 3 | 3162 | no | no | — | #50001 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-markdown-tab-title` | 1 | 3135 | no | no | — | #50018 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `agent_ui/fix-relative-file-links` | 4 | 3037 | no | no | — | #50048 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `clickable-breadcrumbs` | 2 | 2940 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `feat/support-eslint-in-monorepos` | 1 | 2865 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix/parent-numbering-for-indented-list` | 3 | 2719 | no | no | — | #49017 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-diff-keyboard-split-view` | 2 | 2644 | no | no | — | #51457 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-crash-on-mutiple-selections-in-helix-mode` | 1 | 2581 | no | no | — | #51590 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-debugger-not-taking-to-node_modules` | 1 | 2581 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix-git-new-staged-files-stays-untracked` | 2 | 2567 | no | no | — | #51729 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-support-snippet-completions` | 1 | 2474 | no | no | — | #51869 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-tab-switcher-mouse-hover` | 2 | 2204 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix-error-response-max-token-reached` | 3 | 2125 | no | no | — | #50372 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-max-output-token-error` | 1 | 2125 | no | yes | 0 | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix-numbering-for-indented-list` | 11 | 2125 | no | yes | 0 | #52677 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-copilot-thinking-levels` | 1 | 2067 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix-devcontainer-fails-while-using-labels` | 2 | 1971 | no | yes | 0 | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix-dev-container-fails-with-updateRemoteUserUID` | 2 | 1966 | no | yes | 0 | #53084 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-graph-continous-crash` | 2 | 1964 | no | yes | 0 | #53041 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-autosave-on-focus-change-error-when-switching-git-diff` | 2 | 1715 | no | yes | 0 | #53920 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-devcontainer-incorrectly-resolves-incorrect-file-path` | 1 | 1316 | no | yes | 0 | #54749 | CLOSED | closed_pr_unique_or_abandoned | **KEEP_REVIEW** |
| `fix-broken-link-for-zed-release` | 1 | 1271 | no | no | — | — | — | unique_no_pr | **KEEP_REVIEW** |
| `fix/x11-content-size` | 3 | 3474 | no | no | — | #49174 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-commands-remove-indentation` | 4 | 3037 | no | no | — | #50523 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-renaming-html-dots-not-support-dots` | 3 | 3037 | no | no | — | #50373 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-autosave-on-buffer-change-in-multibuffer` | 3 | 2868 | no | no | — | #50686 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/eslint-monorepo-working-directory` | 0 | 2866 | yes | no | — | — | — | fully_on_main | **DELETE_SAFE** |
| `fix-replace-all` | 2 | 2865 | no | no | — | #50852 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-ai-settings` | 5 | 2787 | no | no | — | #50941 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-no-copy-command` | 1 | 2785 | no | no | — | #51191 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/ordered-list-indent-outdent` | 0 | 2694 | yes | no | — | — | — | fully_on_main | **DELETE_SAFE** |
| `fix-outline-filtering-always-select-last-match` | 7 | 2586 | no | no | — | #50594 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-claude-agent-model-reset` | 2 | 2581 | no | no | — | #51587 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-file-rename-on-fuse-based-filesystems` | 1 | 2497 | no | no | — | #51779 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-character-not-encoded-properly` | 1 | 2474 | no | no | — | #51899 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-two-focused-states` | 4 | 2447 | no | no | — | #50827 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `git_ui/fix-diff-clipboard-multibuffer` | 2 | 2434 | no | no | — | #51985 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-highlight-await-as-keyword.control-in-JS/TS/TSX` | 1 | 2358 | no | no | — | #52034 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `git_ui/splittable-editor-diff-view` | 1 | 2332 | no | no | — | #51966 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-wrong-selection-in-commit-panel` | 1 | 2204 | no | yes | 0 | #52673 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/gemini-tool-schema-unsupported-keys` | 1 | 2148 | no | yes | 0 | #52670 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-preserve-settings-during-migrations` | 5 | 2144 | no | yes | 0 | #52676 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-slow-tree-sitter-parsing` | 2 | 2144 | no | yes | 0 | #52674 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `linux/fix-agent-panel-keybindings` | 2 | 2144 | no | yes | 0 | #52672 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/diagnostics-toolbar-hide-inline-assist-when-agent-disabled` | 1 | 2143 | no | yes | 0 | #52706 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-max-token-error-message` | 2 | 2125 | no | yes | 0 | #52724 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-diagnostics-auto-enable` | 6 | 2057 | no | yes | 0 | #52906 | CLOSED | stale_duplicate | **DELETE_SAFE** |
| `fix-diagnostics-toggle` | 6 | 2057 | no | yes | 0 | — | — | stale_duplicate | **DELETE_SAFE** |
| `fix-diagnostics-toggling` | 2 | 2057 | no | yes | 2 | #52907 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/devcontainer-compose-labels` | 2 | 1971 | no | yes | 0 | #53057 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix/duplicating-files-select-only-copy-suffix` | 2 | 1955 | no | yes | 0 | #53146 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-repeated-prompts-in-opencode-acp` | 3 | 1950 | no | yes | 0 | #53216 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `user-configurable-mouse-bindings` | 7 | 1715 | no | yes | 0 | #53889 | CLOSED | stale_duplicate | **DELETE_SAFE** |
| `fix/debugger-start-ignore-save-property` | 3 | 1477 | no | yes | 0 | #53353 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-agent-thread-sidebar-covering-window-buttons` | 1 | 1314 | no | yes | 0 | #54755 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-agent-can-execute-tools-that-are-turned-off` | 1 | 1287 | no | yes | 0 | #54863 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `fix-git-worktree-popup-lists-no-worktree` | 1 | 1238 | no | yes | 0 | #55053 | MERGED | merged_pr_stale | **DELETE_SAFE** |
| `backup/mouse-bindings-v2-before-rewrite` | 2 | 43 | no | no | — | — | — | stale_duplicate | **DELETE_SAFE** |
| `scratch/mouse-bindings-backup` | 2 | 43 | no | no | — | — | — | stale_duplicate | **DELETE_SAFE** |

### Branches with an open PR

- `fix-git-tempalte-do-not-work-in-reote` → Open PR #55490: Support loading Git commit templates when remote (behind main by **1173**, ahead **1)**
- `fix-mcp-servers-in-multi-root-wrokspaces` → Open PR #52849: Fix MCP servers in multi root workspaces (behind main by **2057**, ahead **5)**
- `fix-tab-switcher-random-jumps` → Open PR #52671: Fix tab switcher random jumps (behind main by **2145**, ahead **2)**
- `fix-zoom-pan-not-possible-in-svg-preview` → Open PR #54907: svg_preview: Add zoom and pan support (behind main by **1271**, ahead **2)**
- `mouse-bindings-v2` → Current active work / open PR #55216 (behind main by **7**, ahead **2)**

### Stale duplicates of already-merged work (safe delete)

- `backup/mouse-bindings-v2-before-rewrite` — Superseded by mouse-bindings-v2 (open PR #55216); closed predecessor #53889 _(behind 43, ahead 2)_
- `fix-agent-can-execute-tools-that-are-turned-off` — PR #54863 MERGED 2026-05-05; local tip diverges only because history rewrote / not rebased _(behind 1287, ahead 1)_
- `fix-agent-thread-sidebar-covering-window-buttons` — PR #54755 MERGED 2026-04-24; local tip diverges only because history rewrote / not rebased _(behind 1314, ahead 1)_
- `fix-ai-settings` — PR #50941 MERGED 2026-03-09; local tip diverges only because history rewrote / not rebased _(behind 2787, ahead 5)_
- `fix-autosave-on-buffer-change-in-multibuffer` — PR #50686 MERGED 2026-03-05; local tip diverges only because history rewrote / not rebased _(behind 2868, ahead 3)_
- `fix-character-not-encoded-properly` — PR #51899 MERGED 2026-03-19; local tip diverges only because history rewrote / not rebased _(behind 2474, ahead 1)_
- `fix-claude-agent-model-reset` — PR #51587 MERGED 2026-03-16; local tip diverges only because history rewrote / not rebased _(behind 2581, ahead 2)_
- `fix-commands-remove-indentation` — PR #50523 MERGED 2026-03-12; local tip diverges only because history rewrote / not rebased _(behind 3037, ahead 4)_
- `fix-diagnostics-auto-enable` — Duplicate of merged diagnostics work (#52907) _(behind 2057, ahead 6)_
- `fix-diagnostics-toggle` — Duplicate of merged diagnostics work (#52907) _(behind 2057, ahead 6)_
- `fix-diagnostics-toggling` — PR #52907 MERGED 2026-05-04; local tip diverges only because history rewrote / not rebased _(behind 2057, ahead 2)_
- `fix-file-rename-on-fuse-based-filesystems` — PR #51779 MERGED 2026-03-18; local tip diverges only because history rewrote / not rebased _(behind 2497, ahead 1)_
- `fix-git-worktree-popup-lists-no-worktree` — PR #55053 MERGED 2026-05-05; local tip diverges only because history rewrote / not rebased _(behind 1238, ahead 1)_
- `fix-highlight-await-as-keyword.control-in-JS/TS/TSX` — PR #52034 MERGED 2026-03-23; local tip diverges only because history rewrote / not rebased _(behind 2358, ahead 1)_
- `fix-max-token-error-message` — PR #52724 MERGED 2026-03-30; local tip diverges only because history rewrote / not rebased _(behind 2125, ahead 2)_
- `fix-no-copy-command` — PR #51191 MERGED 2026-03-10; local tip diverges only because history rewrote / not rebased _(behind 2785, ahead 1)_
- `fix-outline-filtering-always-select-last-match` — PR #50594 MERGED 2026-03-16; local tip diverges only because history rewrote / not rebased _(behind 2586, ahead 7)_
- `fix-preserve-settings-during-migrations` — PR #52676 MERGED 2026-03-30; local tip diverges only because history rewrote / not rebased _(behind 2144, ahead 5)_
- `fix-renaming-html-dots-not-support-dots` — PR #50373 MERGED 2026-03-02; local tip diverges only because history rewrote / not rebased _(behind 3037, ahead 3)_
- `fix-repeated-prompts-in-opencode-acp` — PR #53216 MERGED 2026-04-08; local tip diverges only because history rewrote / not rebased _(behind 1950, ahead 3)_
- `fix-replace-all` — PR #50852 MERGED 2026-03-19; local tip diverges only because history rewrote / not rebased _(behind 2865, ahead 2)_
- `fix-slow-tree-sitter-parsing` — PR #52674 MERGED 2026-04-21; local tip diverges only because history rewrote / not rebased _(behind 2144, ahead 2)_
- `fix-two-focused-states` — PR #50827 MERGED 2026-03-19; local tip diverges only because history rewrote / not rebased _(behind 2447, ahead 4)_
- `fix-wrong-selection-in-commit-panel` — PR #52673 MERGED 2026-03-30; local tip diverges only because history rewrote / not rebased _(behind 2204, ahead 1)_
- `fix/debugger-start-ignore-save-property` — PR #53353 MERGED 2026-04-21; local tip diverges only because history rewrote / not rebased _(behind 1477, ahead 3)_
- `fix/devcontainer-compose-labels` — PR #53057 MERGED 2026-04-03; local tip diverges only because history rewrote / not rebased _(behind 1971, ahead 2)_
- `fix/diagnostics-toolbar-hide-inline-assist-when-agent-disabled` — PR #52706 MERGED 2026-04-20; local tip diverges only because history rewrote / not rebased _(behind 2143, ahead 1)_
- `fix/duplicating-files-select-only-copy-suffix` — PR #53146 MERGED 2026-04-08; local tip diverges only because history rewrote / not rebased _(behind 1955, ahead 2)_
- `fix/eslint-monorepo-working-directory` — Tip is ancestor of origin/main with 0 unique commits _(behind 2866, ahead 0)_
- `fix/gemini-tool-schema-unsupported-keys` — PR #52670 MERGED 2026-03-29; local tip diverges only because history rewrote / not rebased _(behind 2148, ahead 1)_
- `fix/ordered-list-indent-outdent` — Tip is ancestor of origin/main with 0 unique commits _(behind 2694, ahead 0)_
- `fix/x11-content-size` — PR #49174 MERGED 2026-02-17; local tip diverges only because history rewrote / not rebased _(behind 3474, ahead 3)_
- `git_ui/fix-diff-clipboard-multibuffer` — PR #51985 MERGED 2026-03-20; local tip diverges only because history rewrote / not rebased _(behind 2434, ahead 2)_
- `git_ui/splittable-editor-diff-view` — PR #51966 MERGED 2026-03-23; local tip diverges only because history rewrote / not rebased _(behind 2332, ahead 1)_
- `linux/fix-agent-panel-keybindings` — PR #52672 MERGED 2026-03-30; local tip diverges only because history rewrote / not rebased _(behind 2144, ahead 2)_
- `scratch/mouse-bindings-backup` — Superseded by mouse-bindings-v2 (open PR #55216); closed predecessor #53889 _(behind 43, ahead 2)_
- `user-configurable-mouse-bindings` — Superseded by mouse-bindings-v2 (open PR #55216); closed predecessor #53889 _(behind 1715, ahead 7)_

### Unique / needs review (kept locally)

- `agent_ui/fix-relative-file-links` — ahead=4 behind=3037 areas=[agent_ui] — Closed PR #50048 without merge; may still have unique commits (ahead=4)
  - PR: #50048 CLOSED https://github.com/zed-industries/zed/pull/50048
  - tip: `7e353ffe1294` fix relative links openn in remote
- `clickable-breadcrumbs` — ahead=2 behind=2940 areas=[editor, image_viewer, language, multi_buffer, outline, outline_panel] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `fe372d49c763` clickable breadcrumbs usig buffers
- `feat/support-eslint-in-monorepos` — ahead=1 behind=2865 areas=[languages] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `7b2a0a6d36d7` feature :  support e eslint in monorepos
- `fix-autosave-on-focus-change-error-when-switching-git-diff` — ahead=2 behind=1715 areas=[workspace] — Closed PR #53920 without merge; may still have unique commits (ahead=2)
  - PR: #53920 CLOSED https://github.com/zed-industries/zed/pull/53920
  - tip: `a6c57780db60` added test & fmt
- `fix-breakpoint-placement-guards` — ahead=3 behind=3162 areas=[editor] — Closed PR #50001 without merge; may still have unique commits (ahead=3)
  - PR: #50001 CLOSED https://github.com/zed-industries/zed/pull/50001
  - tip: `d0aa90cd0db5` optimal fix
- `fix-broken-link-for-zed-release` — ahead=1 behind=1271 areas=[auto_update_ui] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `5519231bc0b1` Fix broken links
- `fix-copilot-thinking-levels` — ahead=1 behind=2067 areas=[language_models] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `6e10166d249e` fix
- `fix-crash-on-mutiple-selections-in-helix-mode` — ahead=1 behind=2581 areas=[vim] — Closed PR #51590 without merge; may still have unique commits (ahead=1)
  - PR: #51590 CLOSED https://github.com/zed-industries/zed/pull/51590
  - tip: `389b2a68a66a` [200~vim: Fix crash when navigating search matches in Helix select mode at end 
- `fix-debugger-not-taking-to-node_modules` — ahead=1 behind=2581 areas=[debugger_ui, project] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `0280dcb4d79f` fix
- `fix-dev-container-fails-with-updateRemoteUserUID` — ahead=2 behind=1966 areas=[dev_container] — Closed PR #53084 without merge; may still have unique commits (ahead=2)
  - PR: #53084 CLOSED https://github.com/zed-industries/zed/pull/53084
  - tip: `57821972ea0c` added tests
- `fix-devcontainer-fails-while-using-labels` — ahead=2 behind=1971 areas=[dev_container, git, git_graph] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `a8269450af2e` fix dev container fails to open when Docker compose fails
- `fix-devcontainer-incorrectly-resolves-incorrect-file-path` — ahead=1 behind=1316 areas=[dev_container] — Closed PR #54749 without merge; may still have unique commits (ahead=1)
  - PR: #54749 CLOSED https://github.com/zed-industries/zed/pull/54749
  - tip: `19005cdd18ff` fix
- `fix-diff-keyboard-split-view` — ahead=2 behind=2644 areas=[git_ui] — Closed PR #51457 without merge; may still have unique commits (ahead=2)
  - PR: #51457 CLOSED https://github.com/zed-industries/zed/pull/51457
  - tip: `fd50e1f1d4b4` added regression test
- `fix-error-response-max-token-reached` — ahead=3 behind=2125 areas=[acp_thread] — Closed PR #50372 without merge; may still have unique commits (ahead=3)
  - PR: #50372 CLOSED https://github.com/zed-industries/zed/pull/50372
  - tip: `19b78e87dc46` Merge branch 'main' into fix-error-response-max-token-reached
- `fix-git-new-staged-files-stays-untracked` — ahead=2 behind=2567 areas=[git_ui] — Closed PR #51729 without merge; may still have unique commits (ahead=2)
  - PR: #51729 CLOSED https://github.com/zed-industries/zed/pull/51729
  - tip: `a89930a19fc8` added a minimal test
- `fix-graph-continous-crash` — ahead=2 behind=1964 areas=[git, git_graph] — Closed PR #53041 without merge; may still have unique commits (ahead=2)
  - PR: #53041 CLOSED https://github.com/zed-industries/zed/pull/53041
  - tip: `9573c4c15b9e` resolve merge conflict and fmt
- `fix-markdown-tab-title` — ahead=1 behind=3135 areas=[agent_ui] — Closed PR #50018 without merge; may still have unique commits (ahead=1)
  - PR: #50018 CLOSED https://github.com/zed-industries/zed/pull/50018
  - tip: `653abec58642` Fix markdown tab title
- `fix-max-output-token-error` — ahead=1 behind=2125 areas=[acp_thread] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `e7f19e1b7394` acp_thread: Clarify max output token error message
- `fix-numbering-for-indented-list` — ahead=11 behind=2125 areas=[editor, keymaps, zed_actions] — Closed PR #52677 without merge; may still have unique commits (ahead=11)
  - PR: #52677 CLOSED https://github.com/zed-industries/zed/pull/52677
  - tip: `41980545984d` fix error
- `fix-support-snippet-completions` — ahead=1 behind=2474 areas=[git_ui, keymaps, snippets_ui] — Closed PR #51869 without merge; may still have unique commits (ahead=1)
  - PR: #51869 CLOSED https://github.com/zed-industries/zed/pull/51869
  - tip: `e686acd7ca79` git_ui: Support snippet completions in commit message editor
- `fix-tab-switcher-mouse-hover` — ahead=2 behind=2204 areas=[language, tab_switcher] — No PR on zed-industries/zed; has unique commits not known-merged
  - tip: `63f3cf991620` tab_switcher: Delay popover to prevent mouse interference on quick switch
- `fix/parent-numbering-for-indented-list` — ahead=3 behind=2719 areas=[editor] — Closed PR #49017 without merge; may still have unique commits (ahead=3)
  - PR: #49017 CLOSED https://github.com/zed-industries/zed/pull/49017
  - tip: `a4aa475ce61c` Merge branch 'main' into fix/parent-numbering-for-indented-list
- `responsive-panel-sizing` — ahead=1 behind=3470 areas=[settings, settings_content, workspace] — Closed PR #49224 without merge; may still have unique commits (ahead=1)
  - PR: #49224 CLOSED https://github.com/zed-industries/zed/pull/49224
  - tip: `110a3c75f71e` feat: implement responsive panel sizing at dock level

## Delete plan executed

The following local branches were classified **DELETE_SAFE** and removed in this health-check pass:

- `backup/mouse-bindings-v2-before-rewrite`
- `fix-agent-can-execute-tools-that-are-turned-off`
- `fix-agent-thread-sidebar-covering-window-buttons`
- `fix-ai-settings`
- `fix-autosave-on-buffer-change-in-multibuffer`
- `fix-character-not-encoded-properly`
- `fix-claude-agent-model-reset`
- `fix-commands-remove-indentation`
- `fix-diagnostics-auto-enable`
- `fix-diagnostics-toggle`
- `fix-diagnostics-toggling`
- `fix-file-rename-on-fuse-based-filesystems`
- `fix-git-worktree-popup-lists-no-worktree`
- `fix-highlight-await-as-keyword.control-in-JS/TS/TSX`
- `fix-max-token-error-message`
- `fix-no-copy-command`
- `fix-outline-filtering-always-select-last-match`
- `fix-preserve-settings-during-migrations`
- `fix-renaming-html-dots-not-support-dots`
- `fix-repeated-prompts-in-opencode-acp`
- `fix-replace-all`
- `fix-slow-tree-sitter-parsing`
- `fix-two-focused-states`
- `fix-wrong-selection-in-commit-panel`
- `fix/debugger-start-ignore-save-property`
- `fix/devcontainer-compose-labels`
- `fix/diagnostics-toolbar-hide-inline-assist-when-agent-disabled`
- `fix/duplicating-files-select-only-copy-suffix`
- `fix/eslint-monorepo-working-directory`
- `fix/gemini-tool-schema-unsupported-keys`
- `fix/ordered-list-indent-outdent`
- `fix/x11-content-size`
- `git_ui/fix-diff-clipboard-multibuffer`
- `git_ui/splittable-editor-diff-view`
- `linux/fix-agent-panel-keybindings`
- `scratch/mouse-bindings-backup`
- `user-configurable-mouse-bindings`

Retained:

- `agent_ui/fix-relative-file-links` (KEEP_REVIEW) — Closed PR #50048 without merge; may still have unique commits (ahead=4)
- `clickable-breadcrumbs` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `feat/support-eslint-in-monorepos` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-autosave-on-focus-change-error-when-switching-git-diff` (KEEP_REVIEW) — Closed PR #53920 without merge; may still have unique commits (ahead=2)
- `fix-breakpoint-placement-guards` (KEEP_REVIEW) — Closed PR #50001 without merge; may still have unique commits (ahead=3)
- `fix-broken-link-for-zed-release` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-copilot-thinking-levels` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-crash-on-mutiple-selections-in-helix-mode` (KEEP_REVIEW) — Closed PR #51590 without merge; may still have unique commits (ahead=1)
- `fix-debugger-not-taking-to-node_modules` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-dev-container-fails-with-updateRemoteUserUID` (KEEP_REVIEW) — Closed PR #53084 without merge; may still have unique commits (ahead=2)
- `fix-devcontainer-fails-while-using-labels` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-devcontainer-incorrectly-resolves-incorrect-file-path` (KEEP_REVIEW) — Closed PR #54749 without merge; may still have unique commits (ahead=1)
- `fix-diff-keyboard-split-view` (KEEP_REVIEW) — Closed PR #51457 without merge; may still have unique commits (ahead=2)
- `fix-error-response-max-token-reached` (KEEP_REVIEW) — Closed PR #50372 without merge; may still have unique commits (ahead=3)
- `fix-git-new-staged-files-stays-untracked` (KEEP_REVIEW) — Closed PR #51729 without merge; may still have unique commits (ahead=2)
- `fix-git-tempalte-do-not-work-in-reote` (KEEP) — Open PR #55490: Support loading Git commit templates when remote
- `fix-graph-continous-crash` (KEEP_REVIEW) — Closed PR #53041 without merge; may still have unique commits (ahead=2)
- `fix-markdown-tab-title` (KEEP_REVIEW) — Closed PR #50018 without merge; may still have unique commits (ahead=1)
- `fix-max-output-token-error` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-mcp-servers-in-multi-root-wrokspaces` (KEEP) — Open PR #52849: Fix MCP servers in multi root workspaces
- `fix-numbering-for-indented-list` (KEEP_REVIEW) — Closed PR #52677 without merge; may still have unique commits (ahead=11)
- `fix-support-snippet-completions` (KEEP_REVIEW) — Closed PR #51869 without merge; may still have unique commits (ahead=1)
- `fix-tab-switcher-mouse-hover` (KEEP_REVIEW) — No PR on zed-industries/zed; has unique commits not known-merged
- `fix-tab-switcher-random-jumps` (KEEP) — Open PR #52671: Fix tab switcher random jumps
- `fix-zoom-pan-not-possible-in-svg-preview` (KEEP) — Open PR #54907: svg_preview: Add zoom and pan support
- `fix/parent-numbering-for-indented-list` (KEEP_REVIEW) — Closed PR #49017 without merge; may still have unique commits (ahead=3)
- `main` (KEEP) — Local tracking branch for origin/main (slightly stale is normal)
- `mouse-bindings-v2` (KEEP) — Current active work / open PR #55216
- `responsive-panel-sizing` (KEEP_REVIEW) — Closed PR #49224 without merge; may still have unique commits (ahead=1)

## Methodology

1. `git fetch origin main` + `git fetch fork`
2. For each local branch: `ahead`/`behind` vs `origin/main`, tip ancestry, fork remote existence, unpushed commit count
3. Cross-ref `gh pr list --author OmChillure --state all` on `zed-industries/zed` by `headRefName`
4. **Tip on main?** uses `git merge-base --is-ancestor <tip> origin/main` (false for most merged PR branches because squash/rebase merge rewrote commits)
5. **Safe delete** = merged PR branch OR superseded duplicate OR tip fully on main; never delete current branch, `main`, or open-PR branches
6. Conflict score = shared paths with #55216 (extra weight for `window.rs` / `key_dispatch.rs`)

## Recommended follow-ups

1. Rebase open PR branches onto latest `origin/main` (they're 1k–2k commits behind)
2. Close or refresh stale open PRs if upstream fixed them independently
3. For KEEP_REVIEW branches: either open a PR, or delete after confirming no unique commits you care about
4. Fast-forward local `main` (`git checkout main && git pull origin main`)
5. Keep iterating on #55216; consider closing #53889 if still listed (already CLOSED)

---

*Report committed to fork branch `chore/branch-health-report` for archival.*

## Post-delete local branch inventory (29 remaining)

```
agent_ui/fix-relative-file-links
clickable-breadcrumbs
feat/support-eslint-in-monorepos
fix-autosave-on-focus-change-error-when-switching-git-diff
fix-breakpoint-placement-guards
fix-broken-link-for-zed-release
fix-copilot-thinking-levels
fix-crash-on-mutiple-selections-in-helix-mode
fix-debugger-not-taking-to-node_modules
fix-devcontainer-fails-while-using-labels
fix-dev-container-fails-with-updateRemoteUserUID
fix-devcontainer-incorrectly-resolves-incorrect-file-path
fix-diff-keyboard-split-view
fix-error-response-max-token-reached
fix-git-new-staged-files-stays-untracked
fix-git-tempalte-do-not-work-in-reote
fix-graph-continous-crash
fix-markdown-tab-title
fix-max-output-token-error
fix-mcp-servers-in-multi-root-wrokspaces
fix-numbering-for-indented-list
fix/parent-numbering-for-indented-list
fix-support-snippet-completions
fix-tab-switcher-mouse-hover
fix-tab-switcher-random-jumps
fix-zoom-pan-not-possible-in-svg-preview
main
mouse-bindings-v2
responsive-panel-sizing
```


# CLAUDE.md — frappe-print_designer (SWE-Pioneers fork)

Changes on top of upstream `frappe/print_designer` (main).

## Arabic i18n
- `print_designer/locale/ar.po` completed to **100% of app-owned strings** (Libyan-appropriate MSA), tagged
  `ai-translated; needs-native-review`. Built/filled via the parent repo's `scripts/i18n` pipeline
  (`generate-pot-file` sync for full doctype/field coverage). See the parent `SWE-Pioneers/frappe`
  `CLAUDE.md` for the pipeline + the runtime `.mo` compile mechanics.
- Desk-embedded designer — RTL via the framework.

## Deploy
Built from `~/build/print_designer-custom` on the VPS (Containerfile repointed to this fork + per-app
`compile-po-to-mo`). Rebuild with `--no-cache`; see the parent `CLAUDE.md` for the `.mo` compile +
persist gotchas.

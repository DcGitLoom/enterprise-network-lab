# Segmentation Policy

> Complete in **Week 3**, enforce with ACLs, then re-enforce at the firewall
> in Week 5. Write the policy first, then make the config match it — not the
> other way around.

Legend: ✅ permit · ❌ deny · ⚠️ permit specific ports only

| From ↓ / To → | employee | servers | iot | voice | guest | internet |
|---|---|---|---|---|---|---|
| **employee** | ✅ | ⚠️ | ❌ | ❌ | ❌ | ✅ |
| **servers** | | | | | | |
| **iot** | | | | | | |
| **voice** | | | | | | |
| **guest** | | | | | | |

## Rationale

<For each ❌ and ⚠️, one line on why. This is the part an interviewer asks
about.>

## Exceptions

| Exception | Justification | Review date |
|---|---|---|
| | | |

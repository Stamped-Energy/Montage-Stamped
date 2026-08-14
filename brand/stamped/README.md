# OpenMontage brand pack — Stamped Energy

**Status: ACTIVE** on this checkout (`config.yaml` → `brand.active: stamped`).

Portable pack for [OpenMontage](https://github.com/calesthio/OpenMontage) / [Montage-Stamped](https://github.com/Stamped-Energy/Montage-Stamped). **Self-contained:** product canon, claims firewall, video DESIGN, C-Vector motion inspiration, playbook, prompts.

Website UI tokens stay on stamped.work (`DESIGN.md` / `styles/theme.css`). This pack does not replace them — it governs OpenMontage video / motion.

Agents: see **Active Brand** in repo-root [`AGENT_GUIDE.md`](../../AGENT_GUIDE.md).

---

## Agent read-order (mandatory)

1. [`context/STAMPED_CONTEXT.md`](context/STAMPED_CONTEXT.md)  
2. [`context/VOICE_AND_CLAIMS.md`](context/VOICE_AND_CLAIMS.md)  
3. [`DESIGN_VIDEO.md`](DESIGN_VIDEO.md) + [`MOTION_LANGUAGE.md`](MOTION_LANGUAGE.md)  
4. Playbook [`../../styles/stamped-industrial.yaml`](../../styles/stamped-industrial.yaml) or [`visual-styles/stamped-industrial.md`](visual-styles/stamped-industrial.md)  
5. Relevant file under [`prompts/`](prompts/)  
6. [`context/sources/`](context/sources/) only when you need depth  

Also skim [`BRAND_BRIDGE.md`](BRAND_BRIDGE.md), [`references/cvector-audit.md`](references/cvector-audit.md), and [`references/homepage-animation-backlog.md`](references/homepage-animation-backlog.md) (site MotionSlot inventory).

---

## Installed layout (this repo)

| Artifact | Location |
|----------|----------|
| Brand pack | `brand/stamped/` (this folder) |
| Style playbook | `styles/stamped-industrial.yaml` |
| Default playbook | `config.yaml` → `brand.default_playbook: stamped-industrial` |
| Pipeline wiring | `stamped-industrial` listed first under `compatible_playbooks.recommended` |

Source copy of the playbook also lives at [`playbooks/stamped-industrial.yaml`](playbooks/stamped-industrial.yaml) — keep in sync if you edit tokens.

### Prompt example

```text
Read brand/stamped using README read-order.
Use playbook stamped-industrial.
Make a 60-second ₹-scored prescriptions explainer for a North India auto-component plant (Band A ICP).
```

---

## Sync note

| Artifact | Upstream | Version pin |
|----------|----------|-------------|
| Master doc | `Research+DOcs/core-product/Stamped_Energy_Master_Document_v1.6.md` | v1.6 Aug 2026 |
| ICP | `Research+DOcs/customer-profile/ICP-North-India-Large-Manufacturer-v3.md` | v3 |
| Website PRODUCT / DESIGN | stamped.work | live |

Refresh `context/sources/` when Master or ICP major-bumps. Distillations may need a short edit pass after.

---

## Folder map

```text
context/           Stamped product + claims + sources
references/        CVector audit + homepage animation backlog
DESIGN_VIDEO.md    Impeccable brand-register video DESIGN
MOTION_LANGUAGE.md Motion physics + signature patterns
BRAND_BRIDGE.md    Website ↔ video token map
playbooks/         Canonical playbook source (synced → styles/)
visual-styles/     visual-style.md + style_prompt_full
prompts/           Production starters
```

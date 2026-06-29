# Viral Product Design Skill

This repository contains a specialized AI agent skill designed to audit, checklist, and guide the development of viral products using the **32 Principles of a Viral Product** framework.

## 📁 Repository Structure

* [viral-product/](file:///c:/Users/indcr/OneDrive/Desktop/prodduct/viral-product)
  * [SKILL.md](file:///c:/Users/indcr/OneDrive/Desktop/prodduct/viral-product/SKILL.md): The core definition of the skill including YAML frontmatter and detailed instructions for AI agents.

## 🚀 About the Skill: `viral-product`

The `viral-product` skill represents a no-BS framework for designing products that people share, remember, and buy. It compiles 32 actionable design, copy, pricing, positioning, and psychological principles.

### Key Focus Areas:
1. **Pricing Strategy**: Hard paywalls, popcorn pricing, and zero free-tier policies.
2. **Copywriting**: Headline simplicity (5th-grade reading level), numbers over adjectives, and stealing customer copy.
3. **Aesthetics & UX**: Minimal color palettes (3 colors max), one idea per screen, and showing the product before explaining it.
4. **Viral Mechanics**: OG image design, shareable footers, and naming conventions.

## ⚙️ How to Install & Use the Skill

AI agents automatically discover and load skills from two primary customization roots. You can install the `viral-product` skill either locally (workspace-level) or globally.

### Option 1: Workspace Installation (Local Project)

To enable this skill for a specific project, place the `viral-product` directory inside your project's `.agents/skills/` directory:

1. Create the `.agents/skills/` folder at the root of your workspace if it doesn't exist.
2. Copy or symlink the `viral-product` directory there.

**Target Structure:**
```text
your-project-root/
└── .agents/
    └── skills/
        └── viral-product/
            └── SKILL.md
```

#### Alternative: Custom/Non-Standard Paths
If you prefer to keep the skill in a shared or custom folder outside `.agents/skills/`, register it in the `.agents/skills.json` file at your project's root:
```json
{
  "entries": [
    { "path": "path/to/viral-product" }
  ]
}
```

---

### Option 2: Global Installation (All Projects)

To make the skill globally available to your agent across all workspaces, install it in the global configurations directory:

- **Windows:** `C:\Users\<YourUsername>\.gemini\config\skills\viral-product`
- **macOS / Linux:** `~/.gemini/config/skills/viral-product`

**Target Structure:**
```text
~/.gemini/config/
└── skills/
    └── viral-product/
        └── SKILL.md
```

---

### Option 3: Installation via `skills.sh` Package Manager (npx)

If your agent environment supports the `skills.sh` registry, you can install the skill automatically using the `skills` CLI wrapper:

```bash
# Using the skills CLI
npx skills add imshreekumarOPS/viral-product-by-marclou

# Shorthand method
npx skill.sh add imshreekumarOPS/viral-product-by-marclou
```

This will automatically pull the skill from the repository and place it into the correct directory for your AI agent.

---

## 🤖 How the Agent Uses This Skill

Once installed and loaded, the agent will automatically discover the `viral-product` skill when analyzing, auditing, or creating product pages. You can trigger it during conversations when:
- Auditing landing page layouts and visual hierarchy.
- Proposing pricing and monetization strategies.
- Drafting high-conversion copywriting and headlines.

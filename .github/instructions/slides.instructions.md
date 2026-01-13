---
applyTo: '**'
---

# Slidev Presentation Guidelines

## Theme Configuration

Always use the theme defined in this project:

```yaml
---
theme: ./
---
```

## Structure Requirements

- **Always** start presentations with the `cover` layout
- **Always** end presentations with the `end` layout. The last slide should always say "Thank you".
- Define layout explicitly for every slide inside the YAML frontmatter block

### Layout Syntax

Layouts MUST be defined inside the YAML frontmatter block (between `---` markers):

**CORRECT:**
```markdown
---
layout: default
---

# Slide Title
Content here
```

**INCORRECT:**
```markdown
---

# Slide Title

layout: default
```

Common layouts: `cover`, `default`, `end`

## Content Guidelines

### Text Limits
- Maximum **30 words** per slide (excluding code examples)
- Code examples do NOT count towards word limit
- Keep text concise - presentations are visual aids, not documents

### Slide Organization
- Break complex topics into multiple slides
- One concept per slide for clarity
- Avoid walls of text - use visuals and diagrams when possible

## Interactive Elements

- Use `<v-clicks>` components to reveal content progressively
- Reveal bullet points one by one to maintain audience focus
- Apply to lists, images, and code blocks for better pacing

## Best Practices

- Prioritize visual hierarchy and white space
- Use consistent formatting throughout
- Ensure readability with appropriate font sizes

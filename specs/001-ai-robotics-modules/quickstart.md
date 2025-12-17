# Quickstart: Physical AI & Humanoid Robotics — Docusaurus Book

## Prerequisites

- Node.js LTS (v18.x or higher)
- npm or yarn package manager
- Git for version control
- Text editor or IDE

## Setup Instructions

### 1. Clone and Initialize Repository
```bash
git clone [repository-url]
cd [repository-name]
npm install
```

### 2. Install Docusaurus
```bash
npm install @docusaurus/core@latest @docusaurus/preset-classic@latest
```

### 3. Create Project Structure
```bash
mkdir -p docs/module-1-ros-2
mkdir -p docs/module-2-digital-twin
mkdir -p docs/module-3-ai-robot-brain
mkdir -p docs/module-4-vision-language-action
mkdir -p static/img
mkdir -p src/components
```

### 4. Initialize Docusaurus Configuration
```bash
npx @docusaurus/init --init-version latest
```

## Development Workflow

### Start Development Server
```bash
npm run start
```
This will start a local development server at http://localhost:3000

### Create New Chapter
1. Create a new Markdown file in the appropriate module directory
2. Add frontmatter with title and description
3. Write content in Markdown format
4. Add APA-style citations in the references section
5. Add the document ID to `sidebars.js`

### Build Static Site
```bash
npm run build
```
This generates the static site in the `build/` directory

### Deploy to GitHub Pages
```bash
npm run deploy
```

## Content Creation Guidelines

### Chapter Structure Template
```markdown
---
title: [Chapter Title]
description: [Brief description of chapter content and objectives]
---

# [Chapter Title]

## Learning Objectives
- Objective 1
- Objective 2
- Objective 3

## Introduction
[Opening content that connects to previous chapter and introduces current topic]

## Main Content
[Detailed content with headings, examples, and code snippets as needed]

## Summary
[Key takeaways and connection to next chapter]

## References
[APA-style citations for sources used in this chapter]
```

### Citation Format
All citations must follow APA 7th edition format:
- Journal articles: Author, A. A. (Year). Title of article. *Title of Periodical*, volume(issue), pages. https://doi.org/xx.xxx/yyyy
- Conference papers: Author, A. A. (Year). Title of paper. *Title of Conference*, pages. Publisher. https://doi.org/xx.xxx/yyyy
- Books: Author, A. A. (Year). *Title of work*. Publisher.

## Quality Checks

### Before Committing
- [ ] Run `npm run build` to verify site builds without errors
- [ ] Verify all internal links work correctly
- [ ] Check that citations follow APA format
- [ ] Confirm chapter meets minimum content requirements
- [ ] Validate that navigation works as expected

### Continuous Integration
- Automated build validation
- Link checking
- Content compliance verification
# Data Model: Physical AI & Humanoid Robotics — Docusaurus Book

## Content Entities

### Module
- **name**: string (e.g., "The Robotic Nervous System (ROS 2)")
- **description**: string (module focus and objectives)
- **chapters**: array of Chapter entities (exactly 3 per module)
- **learningObjectives**: array of strings (what learners will understand)
- **prerequisites**: array of strings (required background knowledge)
- **duration**: number (estimated time to complete in hours)

### Chapter
- **title**: string (chapter name)
- **module**: reference to parent Module
- **position**: number (1-3, defines order within module)
- **content**: string (Markdown content)
- **learningObjectives**: array of strings (specific objectives for this chapter)
- **citations**: array of Citation entities (≥2 per chapter to meet ≥8 per module)
- **examples**: array of Example entities (practical applications)

### Citation
- **id**: string (unique identifier)
- **type**: enum (journal, conference, book, online, report)
- **authors**: array of strings (author names)
- **title**: string (publication title)
- **journal**: string (publication venue)
- **year**: number (publication year)
- **doi**: string (digital object identifier)
- **url**: string (access URL)
- **accessDate**: string (date accessed in YYYY-MM-DD format)

### Example
- **title**: string (example name)
- **description**: string (what the example demonstrates)
- **code**: string (code snippet if applicable)
- **module**: reference to Module
- **chapter**: reference to Chapter

## Navigation Structure

### Sidebar Category
- **label**: string (category name)
- **items**: array of SidebarItem entities
- **collapsible**: boolean (whether section can be collapsed)
- **collapsed**: boolean (initial collapsed state)

### Sidebar Item
- **type**: enum (doc, link, category)
- **label**: string (display name)
- **id**: string (reference to document)
- **href**: string (external link if applicable)

## Validation Rules

### Module Validation
- Each module must have exactly 3 chapters
- Module learning objectives must align with overall specification
- Module duration must be reasonable (2-10 hours per module)

### Chapter Validation
- Each chapter must have ≥2 citations to contribute to module's ≥8 total
- Chapter content must be substantial (minimum 1000 words)
- Chapter learning objectives must be specific and measurable

### Citation Validation
- ≥50% of citations per module must be peer-reviewed
- All citations must be from last 10 years
- Citation format must follow APA style

## State Transitions

### Content Creation Workflow
1. **Draft** → Content is being written
2. **Review** → Content is ready for review
3. **Approved** → Content meets all specification requirements
4. **Published** → Content is available in final documentation

### Quality Gates
- Content must pass build validation
- All citations must be verified
- Navigation must be functional
- Cross-references must be accurate
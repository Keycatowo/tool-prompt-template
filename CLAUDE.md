# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a standalone HTML-based prompt template tool designed for Chinese/Traditional Chinese users. The application is a single-page web application that allows users to:

- Create and edit prompt templates with placeholder variables using `[variable]` syntax
- Fill in placeholder values interactively
- Add formatting requirements through categorized quick-action buttons
- Share templates via URL parameters
- Copy final prompts to clipboard

## Architecture

### Single File Structure
- `index.html` - Complete standalone application containing HTML, CSS, and JavaScript
- No build process, package.json, or external dependencies
- Pure vanilla JavaScript with no frameworks

### Key Components
- **Template Editor**: Modal dialog for creating/editing prompt templates
- **Placeholder System**: Uses `[variable]` syntax for dynamic content insertion
- **Format Categories**: Organized tabs for different types of formatting requirements:
  - Output formats (table, list, JSON, paragraph)
  - Length control (50 words, 100 words, detailed analysis)
  - Structure requirements (bullet points, steps, Q&A)
  - Language style (professional, simple, business, academic)
  - Special requirements (examples, data support, feasibility analysis)
- **Conflict Resolution**: Automatic removal of conflicting format requirements
- **URL Sharing**: Template sharing via URL parameters

### Core Data Structures
- `currentTemplate`: Current template string with placeholders
- `placeholders`: Array of placeholder objects with content and indices
- `filledValues`: Object mapping placeholder indices to user input
- `addedFormats`: Array of selected formatting requirements
- `formatConflicts`: Configuration object defining mutually exclusive format categories

## Development Notes

### Development Commands

#### Local Development Server
```bash
# Using Python (recommended for simple local testing)
python -m http.server 8000

# Using Node.js
npx serve .
```

#### No Build Commands
This is a static HTML file with no build process. Simply open `index.html` in a web browser to run the application.

#### Version Management
- Update version in `package.json`
- Create corresponding changelog file in `changelogs/vX.X.X.md`
- Use semantic versioning (vX.X.X format)
- Create tags on `dev` branch to trigger automated release

### Localization
The application is designed for Traditional Chinese users with Chinese UI text and prompt templates. All user-facing text is in Traditional Chinese.

### Browser Compatibility
Uses modern JavaScript features including:
- ES6 template literals and arrow functions
- Clipboard API with fallback to `document.execCommand`
- CSS Grid and Flexbox for layout

### Key Functions
- `parseTemplate()`: Extracts placeholders from template string
- `renderTemplate()`: Updates display with current state
- `addFormat()`: Manages format conflicts and additions
- `copyResult()`: Generates final prompt and copies to clipboard
- `copyTemplateUrl()`: Creates shareable URL with encoded template
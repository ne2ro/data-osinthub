# 🔍 OSINT Hub Data

> **Community-driven repository of OSINT tools and resources**
> Curated collection of Open Source Intelligence tools organized by category

[![Validation](https://img.shields.io/badge/validation-passing-brightgreen)](https://github.com/ne2ro/data-osinthub/actions)
[![Contributors](https://img.shields.io/badge/contributors-welcome-blue)](#-contribute)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

> 🌐 Explore the live OSINT Hub directory at [osinthub.ad0.dev](https://osinthub.ad0.dev/)

---

## 📁 Repository Structure

```
├── 📄 tools.json         # Core categories and tools 
└── 📋 schema/            # JSON schemas for validation
    └── tools.schema.json
```

### 🔧 File Descriptions

| File | Status | Description |
|------|--------|-------------|
| `tools.json` | **Required** | Main database of OSINT tools organized by categories |

---

## 🤝 Contribute

We welcome contributions from the OSINT community! Here's how you can help:

### 📝 Quick Start
1. **Fork** this repository
2. **Edit** `tools.json`
3. **Open** a Pull Request
4. **Wait** for automated validation to pass

> 💡 **Tip**: All submissions are automatically validated through our CI pipeline

### ✅ Local Validation (Optional)

Want to test your changes before submitting? Follow these steps:

```bash
# 1. Install validation tools
npm i -D ajv-cli@5

# 2. Validate your changes
npx ajv validate -s schema/tools.schema.json -d tools.json --all-errors
```

---

## 📊 Data Schema

### 🛠️ Tool Object
```json
{
  "name": "Tool Name",
  "url": "https://example.com"
  // Optional overrides:
  // "description": "Brief description",
  // "icon": "https://example.com/favicon.ico"
}
```

### 📂 Category Object
```json
{
  "category": "Category Name",
  "tools": [
    // Array of tool objects
  ]
}
```

---

## 💡 Best Practices

### ✏️ Writing Guidelines
- **Descriptions**: Only include if they add clear value beyond the tool name (otherwise omit)
- **Icons**: Usually omit — the UI auto‑generates favicons from the tool domain. Only set `icon` to override.
  - Do not use third‑party proxies; if needed, use a direct image URL (e.g., the site's real favicon).
- **URLs**: Ensure all links are active and lead to canonical pages; remove tracking params

### 🎯 Quality Standards
- ✅ Verify tool functionality before adding
- ✅ Use clear, descriptive names
- ✅ Categorize appropriately
- ✅ Test all URLs

---

## 🚀 Getting Started

1. **Browse** the `tools.json` file to see existing categories and tools
2. **Identify** gaps or new tools to add
3. **Follow** the schema structure
4. **Submit** your contribution via Pull Request

---

## 💡 Best Practices

### 🎯 Tool Selection Criteria
- **Relevance**: Tool must serve a legitimate OSINT purpose
- **Functionality**: Tool must be actively maintained and functional
- **Documentation**: Clear documentation available (if applicable)
- **Accessibility**: Tool should be publicly accessible without login requirements

### 📝 Submission Guidelines
- **Unique Tools**: Avoid duplicate submissions of existing tools
- **Categorization**: Place tools in the most appropriate category
- **Descriptions**: Keep descriptions concise and informative
- **URLs**: Use direct links to tools, not through proxies or aggregators

### 🔒 Security Considerations
- **Verification**: Ensure tools are safe and from reputable sources
- **Privacy**: Avoid tools that collect excessive user data
- **Legality**: Only include tools that can be used legally

---

## 🤝 Community Guidelines

### 📥 Submitting New Tools
1. **Check** if the tool already exists in the repository
2. **Verify** the tool meets our quality standards
3. **Create** a fork of this repository
4. **Add** your tool to the appropriate category
5. **Test** your changes locally using the validation script
6. **Open** a pull request with a clear description

### 🐛 Reporting Issues
- **Broken Links**: Report tools that are no longer accessible
- **Wrong Categorization**: Suggest better categories for existing tools
- **Missing Tools**: Recommend tools that should be included
- **Data Errors**: Report incorrect information in tool descriptions

### 💬 Feature Requests
- **New Categories**: Suggest new categories for better organization
- **Schema Improvements**: Recommend changes to the data structure
- **Validation Rules**: Propose additional validation criteria

---

## 📚 Data Usage

The OSINT Hub data is used by:
- [osinthub.ad0.dev](https://osinthub.ad0.dev) - Main directory interface
- Various OSINT tools and platforms
- Security researchers and analysts worldwide
- Academic institutions and training programs

### 📄 Data Format
The data is provided in JSON format for easy integration:
- **Real-time Updates**: The latest data is always available via GitHub
- **Version Control**: Track changes and contributions through Git
- **API Access**: Direct access to the JSON data for custom implementations

---

## 💖 Support the Project

Help keep the OSINT Hub data project maintained and freely accessible to everyone.

### 💰 Cryptocurrency Donations
- **Bitcoin**: `bc1qddykxzypgnqa3rhyqhc63c7kr8hy52jg4fhgac`
- **Ethereum**: `0x9919fA5E01cBC3aed8cffAfFF4C496B33Ab87f8F`
- **Litecoin**: `ltc1qtfydnyv46smg5ped00e7sjn4nayf53tfh2gm8m`


## 🙏 Acknowledgments

Thanks to all contributors who help maintain and expand this valuable OSINT resource!

---

<div align="center">

**[⭐ Star this repo](https://github.com/ne2ro/data-osinthub) | [🍴 Fork it](https://github.com/ne2ro/data-osinthub/fork) | [📝 Contribute](#-contribute)**

</div>

# Apple App Store ASO Optimization Skill

A comprehensive Claude Code skill for generating optimized Apple App Store metadata with ASO (App Store Optimization) best practices, competitive analysis, and automated validation.

## 🎯 What This Skill Does

This skill transforms Claude Code into an ASO expert that can:

- **Analyze app concepts** and generate optimized App Store metadata
- **Validate character limits** automatically against Apple's requirements
- **Provide competitive analysis** insights using proven ASO strategies
- **Recommend screenshot storyboards** with caption optimization
- **Apply 2025 algorithm updates** including screenshot caption OCR indexing

## 📋 Features

### Metadata Optimization
- App Name (30 chars) - Highest ranking weight
- Subtitle (30 chars) - Second strongest ranking factor
- Promotional Text (170 chars) - Conversion optimization
- Description (4,000 chars) - Not indexed, purely for conversion
- Keywords (100 chars) - Hidden but indexed field
- What's New (4,000 chars) - Update messaging

### Automated Validation
Python script validates all metadata against Apple's strict character limits with clear ✅/❌ indicators and remaining character counts.

### Comprehensive Knowledge Base
47KB of ASO best practices including:
- June 2025 screenshot caption OCR algorithm update
- Metadata hierarchy and indexing rules
- Competitive analysis frameworks
- Rating optimization strategies
- Localization guidance
- A/B testing recommendations

### Screenshot Strategy
- Caption optimization for new OCR indexing
- A.I.D.A. framework recommendations
- Visual content best practices
- Localization considerations

## 🚀 Installation

### Option 1: Direct Install (Recommended)

1. Download the latest release `.zip` file
2. Extract to your Claude Code skills directory:
   ```bash
   unzip app-store-aso.zip -d ~/.claude/skills/
   ```
3. Restart Claude Code (if currently running)

### Option 2: Git Clone

```bash
cd ~/.claude/skills/
git clone https://github.com/timbroddin/app-store-aso-skill.git app-store-aso
```

### Verify Installation

The skill structure should look like:
```
~/.claude/skills/app-store-aso/
├── SKILL.md                          # Main skill instructions
├── README.md                         # This file
├── scripts/
│   └── validate_metadata.py         # Validation script
└── references/
    └── aso_learnings.md             # Comprehensive ASO knowledge base
```

## 💡 Usage

The skill activates automatically when you ask Claude Code about App Store optimization. Simply describe your app and request ASO help:

### Example Queries

**Basic optimization:**
```
"I have an iOS meditation app called 'CalmSpace'.
Help me optimize the App Store metadata."
```

**With context:**
```
"This is a fitness tracking app for runners.
I've added a new social feature and marathon training plans.
Generate optimized metadata and screenshot recommendations."
```

**Metadata review:**
```
"Review my current App Store listing:
Title: FitTrack - Run & Workout
Subtitle: GPS Running & Fitness Log
Keywords: running,tracker,fitness,workout,gps
Optimize this for better rankings."
```

### Output Format

Claude will provide:

1. **📱 App Metadata Recommendations**
   - Optimized title, subtitle, promotional text
   - Strategic keyword list
   - Compelling description

2. **✅ Validation Results**
   - Character count checks against limits
   - Clear pass/fail indicators
   - Remaining character counts

3. **🎯 Competitive Analysis**
   - Positioning recommendations
   - Keyword opportunities
   - Market insights

4. **📸 Screenshot Storyboard Strategy**
   - Ordered screenshot recommendations
   - Caption optimization for OCR indexing
   - Visual messaging hierarchy

## 🛠️ Validation Script

The included Python script can also be run manually:

### Interactive Mode
```bash
python ~/.claude/skills/app-store-aso/scripts/validate_metadata.py
```

### Command-Line Mode
```bash
python ~/.claude/skills/app-store-aso/scripts/validate_metadata.py \
  --app-name "My Amazing App" \
  --subtitle "The Best App for Everything" \
  --keywords "app,best,amazing,everything,awesome"
```

## 📊 Apple App Store Character Limits

| Field | Limit | Indexed? | Impact |
|-------|-------|----------|--------|
| App Name | 30 chars | ✅ Yes | Highest ranking weight |
| Subtitle | 30 chars | ✅ Yes | Second strongest |
| Promotional Text | 170 chars | ❌ No | Conversion only |
| Description | 4,000 chars | ❌ No | Conversion only |
| Keywords | 100 chars | ✅ Yes | Significant ranking |
| What's New | 4,000 chars | ❌ No | Update messaging |
| Screenshot Captions | Variable | ✅ Yes | NEW in June 2025 |

## 🆕 What's New in 2025

### June 2025 Algorithm Update
Apple deployed OCR technology to extract and index screenshot captions for the first time since 2017. This skill includes:

- Caption optimization strategies for OCR readability
- High-contrast text recommendations
- Keyword reinforcement techniques
- Visual hierarchy best practices

### Other 2025 Changes
- Elimination of new app boost
- Custom Product Pages for organic keywords
- Enhanced in-app event indexing
- 4-week update cycle optimization

## 🎓 ASO Best Practices Included

- **Metadata Hierarchy**: Title > Subtitle > Screenshot Captions > Keywords
- **No Duplication**: Each keyword should appear only once across title/subtitle/keywords
- **Update Frequency**: Every 2-4 weeks minimum
- **Rating Target**: 4.5+ stars for optimal visibility
- **Localization**: 35% average impression increase
- **A/B Testing**: Product Page Optimization strategies

## 🤝 Contributing

Contributions welcome! Areas for improvement:

- Additional ASO research and case studies
- More validation checks (keyword density, etc.)
- Screenshot template generators
- Competitor analysis automation
- Localization tools

## 📄 License

MIT License - see LICENSE file for details

## 🙏 Acknowledgments

Built using the [Claude Code Skill Creator](https://github.com/anthropics/claude-code) framework.

ASO knowledge compiled from industry research, official Apple documentation, and analysis from leading ASO platforms.

## 📞 Support

- **Issues**: Report bugs or request features via [GitHub Issues](https://github.com/timbroddin/app-store-aso-skill/issues)
- **Discussions**: Ask questions in [GitHub Discussions](https://github.com/timbroddin/app-store-aso-skill/discussions)

## 🔗 Resources

- [Apple App Store Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)
- [App Store Connect Help](https://help.apple.com/app-store-connect/)
- [Product Page Optimization](https://developer.apple.com/app-store/product-page-optimization/)
- [Claude Code Skills Documentation](https://docs.claude.com/claude-code)

---

**Made with ❤️ for the Claude Code community**

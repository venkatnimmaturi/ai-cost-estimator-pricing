# AI Cost Estimator - Community Pricing Data

This repository maintains up-to-date pricing information for major AI API providers used by the [AI Cost Estimator](https://your-site-url.com) tool.

## 🎯 Purpose

Keep AI API pricing data current through community contributions. When providers update their pricing, anyone can submit a PR to update this data.

## 📋 Current Providers

- **Claude** (Anthropic)
- **GPT-4** (OpenAI) 
- **Gemini** (Google AI)

## 🔄 How to Update Pricing

### When to Update

Submit a PR when you notice:
- Price changes on official provider websites
- New models added
- Pricing structure changes

### How to Update

1. Fork this repository
2. Edit `pricing.json`:
   - Update the relevant provider pricing
   - Increment the `version` number (e.g., 1.0 → 1.1)
   - Update `last_updated` to current date (YYYY-MM-DD)
   - Add entry to `changelog` array
3. Submit a Pull Request with:
   - Link to official pricing page showing the change
   - Brief description of what changed

### Example PR Description

```
Update Claude Sonnet 4 pricing

- Input: $3.00 → $2.50 per 1M tokens
- Source: https://www.anthropic.com/pricing
- Verified: 2025-02-20
```

## 📊 JSON Structure

```json
{
  "last_updated": "YYYY-MM-DD",
  "version": "X.Y",
  "changelog": [...],
  "providers": {
    "provider_key": {
      "name": "Model Name",
      "input": 0.00,
      "output": 0.00,
      "imageTokens": 0,
      "source": "https://...",
      "notes": "Additional context"
    }
  }
}
```

## ✅ Verification Process

Before merging, PRs are checked for:
- [ ] Version number incremented
- [ ] Date updated
- [ ] Changelog entry added
- [ ] Source link provided
- [ ] Pricing matches official source

## 🔗 Official Pricing Sources

- **Anthropic Claude**: https://www.anthropic.com/pricing
- **OpenAI GPT-4**: https://openai.com/api/pricing/
- **Google Gemini**: https://ai.google.dev/pricing

## 📝 Notes

- All prices in USD per 1 million tokens
- Image token calculations are approximate/average
- Last verified date indicates when pricing was confirmed accurate
- Community members are encouraged to verify monthly

## 🤝 Contributing

We welcome contributions! Please:
- Verify pricing from official sources
- Keep formatting consistent
- Add clear commit messages
- Link to official announcements when available

## 📜 License

This data is maintained by the community and freely available for use. Pricing information is sourced from official provider documentation.

---

**Maintained by the community • Used by AI Cost Estimator**

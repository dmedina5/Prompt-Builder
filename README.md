# Cover Whale - AI Prompt Builder (The Prompt Perfector)

Interactive prompt building tool accessible only to @coverwhale.com email addresses.

## 🔒 Authentication

This GitHub Pages site uses OAuth 2.0 authentication via Google to ensure only Cover Whale employees can access the tool.

### How it Works:
1. User visits the page
2. Prompted to sign in with Google
3. Email domain verified (@coverwhale.com required)
4. JWT token issued and stored
5. Interactive prompt builder displayed

## ✨ Features

### Simple Mode:
- Quick 3-field form for everyday tasks
- Role selection (8 insurance-specific roles)
- Task description
- Output format selection

### Advanced Mode:
- Full CRISP Framework implementation
- Context → Role → Instruction → Specifics → Preferences
- Professional prompt structuring
- Best practices built-in

### Reality Filter:
- Toggle on/off
- Adds confidence scoring requirements
- Verification labels for unverified content
- Critical for important decisions

### Pre-loaded Examples:
- Analyze trucking submission
- Review loss run patterns
- Draft broker communication

### Additional Features:
- Copy to clipboard
- Reset form
- Mode switching
- Mobile responsive
- Cover Whale branding

## 📁 Files

- `index.html` - Authentication wrapper and login page
- `builder.html` - The actual AI Prompt Builder tool
- `README.md` - This file

## 🚀 Deployment

### Prerequisites:
- GitHub account (dmedina5)
- Vercel deployment of `coverwhale-auth` (already set up)
- GitHub Pages enabled

### Deploy Steps:

1. **Create GitHub Repository**
```bash
# Repository name: prompt-builder
# Public visibility required for GitHub Pages
```

2. **Push Code**
```bash
git add .
git commit -m "Initial commit: Protected AI Prompt Builder"
git remote add origin https://github.com/dmedina5/prompt-builder.git
git branch -M main
git push -u origin main
```

3. **Enable GitHub Pages**
- Go to Settings → Pages
- Source: Deploy from main branch
- Root directory
- Save

4. **Access URL**
```
https://dmedina5.github.io/prompt-builder/
```

## 🔧 Configuration

The authentication points to:
- Auth API: `https://coverwhale-auth.vercel.app`
- Allowed domain: `@coverwhale.com`
- Token expiration: 24 hours

## 🧪 Testing

To test authentication:
1. Visit the page in incognito mode
2. Click "Sign in with Google"
3. Use a @coverwhale.com email
4. Verify builder loads
5. Test Simple Mode
6. Test Advanced Mode
7. Test Reality Filter toggle
8. Test pre-loaded examples
9. Refresh page - should remain authenticated

## 🔄 Updating the Builder

To update the builder tool:
1. Edit `builder.html` locally
2. Commit and push to GitHub
3. GitHub Pages will automatically redeploy
4. No authentication changes needed

## 🛡️ Security Features

- ✅ Google OAuth 2.0 authentication
- ✅ Email domain verification (@coverwhale.com only)
- ✅ JWT tokens with expiration
- ✅ Secure token storage (localStorage)
- ✅ Token verification on every load
- ✅ HTTPS only (GitHub Pages)

## 📝 Usage Instructions

### For Users:

**Simple Mode (Beginners):**
1. Select a role (e.g., "Underwriter")
2. Describe what you need help with
3. Choose output format
4. Copy the generated prompt
5. Paste into ChatGPT, Claude, or Copilot

**Advanced Mode (Experienced):**
1. Click "Advanced Mode" button
2. Fill in CRISP Framework fields:
   - Context: Background information
   - Role: Who should AI be?
   - Instruction: What specific task?
   - Specifics: Details and constraints
   - Preferences: Output format and style
3. Toggle Reality Filter if needed (for critical decisions)
4. Copy and use the comprehensive prompt

**Pre-loaded Examples:**
1. Click any example button at bottom
2. Review the pre-filled fields
3. Modify as needed
4. Copy and use

## 🔗 Integration with AI Adoption Page

### Option 1: Direct Link (Recommended)
```markdown
## AI Tools:

- ✨ [Interactive Prompt Builder](https://dmedina5.github.io/prompt-builder/)
  *Internal tool - requires @coverwhale.com authentication*
```

### Option 2: Embed in iframe
```html
<iframe
  src="https://dmedina5.github.io/prompt-builder/"
  width="100%"
  height="950px"
  style="border: 2px solid #6B4E8C; border-radius: 8px;">
</iframe>
```

### Option 3: Combine with Master Guide
```markdown
## Prompt Engineering Resources:

- 📖 [Master Prompt Engineering Guide](https://dmedina5.github.io/prompt-engineering-guide/)
- ✨ [Interactive Prompt Builder](https://dmedina5.github.io/prompt-builder/)

Both tools require @coverwhale.com authentication
```

## 🐛 Troubleshooting

**Issue**: "Access Denied" message
- **Solution**: Must use @coverwhale.com email

**Issue**: Stuck on login screen
- **Solution**: Check browser console, verify Vercel auth is running

**Issue**: Token expired
- **Solution**: Automatic re-login prompt after 24 hours

**Issue**: Builder doesn't load
- **Solution**: Verify `builder.html` exists in repository

**Issue**: Copy to clipboard doesn't work
- **Solution**: Browser security in iframes - users can manually select text

**Issue**: Examples don't load
- **Solution**: Check browser console for JavaScript errors

**Issue**: Mode switching broken
- **Solution**: Clear browser cache, refresh page

## 👥 Access Management

Currently, access is granted to any @coverwhale.com email. To restrict further:
1. Maintain whitelist in Vercel auth backend
2. Check against specific email addresses
3. Implement role-based access if needed

## 📊 Features Breakdown

### Roles Available:
1. Underwriter (Trucking Insurance)
2. Insurance Communicator
3. Data Analyst (Insurance)
4. Coverage Specialist
5. Regulatory Specialist
6. Claims Specialist
7. HR Professional
8. Career Coach

### Output Formats:
1. Prioritized List
2. Bullet Points
3. Email Draft
4. Step-by-Step Plan
5. Comparison Table
6. Detailed Summary
7. Short Summary

### Pre-loaded Examples:
1. **Submission Analysis**: Reviews new trucking submission with fleet details
2. **Loss Run Review**: Analyzes claim patterns for renewals
3. **Broker Email**: Drafts professional request for additional info

## 🎯 Learning Path

1. **Start with Simple Mode** - Get comfortable with basic prompts
2. **Try Examples** - See how professional prompts are structured
3. **Graduate to Advanced Mode** - Learn CRISP Framework
4. **Add Reality Filter** - For critical underwriting decisions
5. **Master Prompt Engineering** - Refer to Master Guide

## 🔗 Related Resources

- **Master Prompt Engineering Guide**: https://dmedina5.github.io/prompt-engineering-guide/
- **CoverWhale Auth Backend**: https://coverwhale-auth.vercel.app
- **AI Adoption Page**: The Harbor (Google Sites)

---

**Maintained by**: Daniel Medina (Manager of Core Systems)
**Last Updated**: January 2026
**Status**: Production Ready
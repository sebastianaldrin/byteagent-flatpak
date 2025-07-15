# Flathub Submission Steps

## ✅ What's Done

1. **Created Flatpak repository** - All files are ready in `byteagent-flatpak/`
2. **Working Flatpak manifest** - Tested and working locally
3. **Required metadata files** - Desktop entry and AppStream metadata
4. **Git repository initialized** - Ready for GitHub

## 🚀 Next Steps (YOU need to do these)

### Step 1: Create GitHub Release

1. **Go to your main ByteAgent repository**
2. **Create a release** (v1.0.0)
3. **Upload the Linux build** as `byteagent-linux-v1.0.0.tar.gz`
   - This should contain the entire `build/flutter/build/linux/x64/release/bundle` directory
   - Plus `src/assets/icon-512.png`

### Step 2: Get SHA256 hash

```bash
# After uploading the release, download it and get the hash:
wget https://github.com/aldrin-ai/byte-agent/releases/download/v1.0.0/byteagent-linux-v1.0.0.tar.gz
sha256sum byteagent-linux-v1.0.0.tar.gz
```

### Step 3: Update the manifest

Edit `com.byteagent.ByteAgent.yml` and replace:
```yaml
sha256: # This will be filled when you create the release
```

With the actual hash:
```yaml
sha256: abc123def456... # The actual hash from step 2
```

### Step 4: Create GitHub repository

1. **Create a new repository** called `byteagent-flatpak`
2. **Push this directory** to that repository:

```bash
cd byteagent-flatpak
git remote add origin https://github.com/aldrin-ai/byteagent-flatpak.git
git push -u origin master
```

### Step 5: Submit to Flathub

1. **Fork the Flathub repository**: https://github.com/flathub/flathub
2. **Create a pull request** with your `byteagent-flatpak` repository
3. **Title**: "Add com.byteagent.ByteAgent"
4. **Description**: "ByteAgent - AI Desktop Assistant with 64+ Professional Tools"

### Step 6: Wait for approval

- Flathub reviewers will test your app
- They may ask for changes
- Usually takes 1-2 weeks
- Once approved, your app appears in all Linux app stores!

## 📋 Checklist

- [ ] Create GitHub release with Linux build
- [ ] Get SHA256 hash and update manifest
- [ ] Create `byteagent-flatpak` repository
- [ ] Push files to GitHub
- [ ] Submit pull request to Flathub
- [ ] Respond to any reviewer feedback

## 🎯 Benefits After Approval

- **Automatic discovery** by millions of Linux users
- **One-click installation** on all major Linux distributions
- **Professional app store presence**
- **Automatic updates** for users
- **SEO benefits** and increased visibility

## 🔗 Links

- [Flathub](https://flathub.org)
- [Flathub GitHub](https://github.com/flathub/flathub)
- [Flatpak Documentation](https://docs.flatpak.org)
- [Flathub Submission Guide](https://github.com/flathub/flathub/wiki/App-Submission)

---

**The hard work is done!** The Flatpak works perfectly - now it's just a matter of following these steps to get it on the official store. 🚀
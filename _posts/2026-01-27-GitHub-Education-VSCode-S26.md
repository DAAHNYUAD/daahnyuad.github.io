---
title: "GitHub Education, VSCode Setup, and Customizing Minimal Mistakes S26"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - lab
  - S26
  - GitHub Education
  - VSCode
  - Github Pages
---

## Getting Started with GitHub Education and Customizing Your Site

Here we look at three important steps to getting on track for [Distant Coding](https://anastasiasalter.net/DistantCoding/transcript.html): verifying your GitHub Education activation, setting up VSCode with your GitHub Education account, and making simple customizations to your Minimal Mistakes template.

<!--more-->

### Part 1: Confirming Your GitHub Education Status

GitHub Education provides free features for students, including unlimited private repositories and access to developer tools for their GitHub account.

**How to verify your GitHub Education is activated:**

> Remember that some interfaces change with time and the exact naming can change without notice. 

1. Log into your GitHub account at [github.com](https://github.com)
2. Click your profile icon in the top-right corner and select `Settings`.
3. In the left sidebar, click `Billing and licensing`
4. Look for a section titled `Education benefits`
5. You should see a message confirming your academic status has been verified and your benefits are active, along with an expiration date
6. Alternatively, you can check your account by visiting [github.com/students](https://github.com/students) and signing in—you'll see a checkmark if your benefits are active

If your GitHub Education is not yet activated, you can apply at the GitHub Education page by providing proof of your student status (student ID, enrollment verification, or .edu email address). You need to be on campus when you make the application and allow your location to be verified. 

### Part 2: Setting Up VSCode with GitHub Education

Once you have your GitHub Education account activated, you can use VSCode as your primary editor and integrate it directly with GitHub.

**Steps to connect VSCode to GitHub:**

1. **Install VSCode** from [code.visualstudio.com](https://code.visualstudio.com/) if you haven't already
2. **Install the GitHub Copilot extension** (optional, but included free with GitHub Education):
   - Open VSCode and go to the Extensions panel (Ctrl+Shift+X on Windows/Linux, Cmd+Shift+X on Mac)
   - Search for "GitHub Copilot" and click **Install**
3. **Install the GitHub Pull Requests and Issues extension:**
   - Search for "GitHub Pull Requests and Issues" in Extensions and install it
4. **Sign in to GitHub from VSCode:**
   - Press Ctrl+Shift+P (or Cmd+Shift+P on Mac) to open the Command Palette
   - Type "GitHub: Sign in" and press Enter
   - Follow the prompts to authenticate with your GitHub account
5. **Clone your repository:**
   - Open the Command Palette and type "Git: Clone"
   - Paste your repository URL (e.g., `https://github.com/yourusername/yourusername.github.io`)
   - Choose a local folder to clone to

Now you can edit files directly in VSCode and push changes to GitHub without needing GitHub Desktop!

### Part 3: Simple Customizations to Minimal Mistakes

The Minimal Mistakes template is highly customizable. Here are some simple changes you can make to personalize your site:

**1. Update Site Title and Description**

Edit the `_config.yml` file in your repository:

```yaml
title: Your Site Title Here
description: A brief description of your site
url: "https://yourusername.github.io"
```

**2. Customize the Navigation Menu**

Edit `_data/navigation.yml` to add links:

```yaml
main:
  - title: "Posts"
    url: /
  - title: "Categories"
    url: /categories/
  - title: "Tags"
    url: /tags/
  - title: "About"
    url: /about/
```

**3. Add a Custom Theme Color**

In `_config.yml`, you can specify a skin (built-in color scheme):

```yaml
minimal_mistakes_skin: "default" # other options: air, aqua, contrast, dark, dirt, neon, mint, plum, sunrise
```

**4. Update Your Author Information**

In `_config.yml`, find the `author:` section and update:

```yaml
author:
  name: "Your Name"
  avatar: "/assets/images/profile.jpg"
  bio: "Your bio here"
  location: "Your location"
  email: your.email@example.com
  links:
    - label: "Website"
      icon: "fas fa-fw fa-link"
      url: "https://yourwebsite.com"
    - label: "GitHub"
      icon: "fab fa-fw fa-github"
      url: "https://github.com/yourusername"
```

**5. Enable Comments (Optional)**

In `_config.yml`, you can enable Disqus comments:

```yaml
comments:
  provider: "disqus"
  disqus:
    shortname: "your-disqus-shortname"
```

**Pushing Your Changes:**

After making edits in VSCode:

1. Open the Source Control panel (Ctrl+Shift+G or Cmd+Shift+G)
2. Review your changes
3. Enter a commit message (e.g., "Update site title and navigation")
4. Click the checkmark to commit
5. Click **Publish Branch** or **Sync** to push to GitHub

Your site will automatically rebuild within a few minutes. You can check the status in your repository's **Actions** tab on GitHub.

### Next Steps

With GitHub Education activated, VSCode set up, and your site customized, you're ready to start creating content! In future posts, we'll explore creating pages, organizing posts by categories, and more advanced customizations.

Enjoy building your portfolio site!

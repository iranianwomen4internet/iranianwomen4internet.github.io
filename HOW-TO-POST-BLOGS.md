# How to Post Blogs

This guide explains how collaborators can easily add new blog posts to the website.

## Quick Steps

1. **Open the blog posts file**: Navigate to `assets/data/blog-posts.json`
2. **Copy the template**: Use the template in `assets/data/blog-post-template.json`
3. **Add your post**: Insert your new post at the beginning of the array
4. **Commit your changes**: The blog will automatically update

## Detailed Instructions

### Step 1: Prepare Your Blog Post

Before you start, have ready:
- Your blog post title
- Your name (as you want it to appear)
- Your content (written in plain text)
- Optional: 2-5 relevant tags

### Step 2: Edit the Blog Posts File

1. Open `assets/data/blog-posts.json` in any text editor
2. Copy the template from `assets/data/blog-post-template.json`
3. Add your new post **at the very beginning** of the array (right after the opening `[`)

### Step 3: Fill Out Your Post

Replace the template values with your content:

```json
{
  "title": "My Amazing Blog Post",
  "author": "Your Name",
  "date": "2024-03-23",
  "content": "This is the first paragraph of my blog post.\n\nThis is the second paragraph. Notice the double \\n between paragraphs.\n\nYou can write as many paragraphs as you need.",
  "tags": ["internet freedom", "human rights", "technology"]
}
```

**Important formatting notes:**
- **Date format**: Use YYYY-MM-DD (e.g., "2024-03-23")
- **Paragraphs**: Use `\n\n` (double backslash-n) to separate paragraphs
- **Quotes**: If you need quotation marks in your content, use `\"` instead of `"`
- **Commas**: Don't forget the comma after your post's closing `}` (except for the last post in the array)

### Step 4: Example of Adding a New Post

Here's what `blog-posts.json` should look like after adding a new post:

```json
[
  {
    "title": "New Post Title",
    "author": "Your Name",
    "date": "2024-03-23",
    "content": "Your new blog post content here.\n\nSecond paragraph.",
    "tags": ["tag1", "tag2"]
  },
  {
    "title": "Welcome to Our Blog",
    "author": "Iranian Women's Coalition",
    "date": "2024-03-23",
    "content": "Welcome to the Iranian Women's Coalition for Internet Freedom blog!...",
    "tags": ["welcome", "internet freedom", "digital rights"]
  }
]
```

### Step 5: Test Your Changes

1. Save the file
2. Open `blog.html` in a web browser
3. Check that your post appears at the top
4. Verify formatting looks correct

### Step 6: Commit Your Changes

If using git:
```bash
git add assets/data/blog-posts.json
git commit -m "Add new blog post: [Your Title]"
git push
```

## Tips for Writing Good Blog Posts

### Content Guidelines
- **Keep it relevant**: Focus on internet freedom, digital rights, or coalition updates
- **Be clear and concise**: Write in accessible language
- **Use paragraphs**: Break up long text for easier reading
- **Add context**: Explain technical terms or background information

### Tag Suggestions
Use relevant tags to help categorize your posts:
- `internet freedom`
- `digital rights`
- `censorship`
- `surveillance`
- `human rights`
- `coalition updates`
- `news`
- `analysis`
- `education`
- `technology`

### Content Ideas
- Updates on coalition activities
- Analysis of internet freedom issues
- Educational content about digital rights
- News commentary
- Personal stories (with permission)
- Technical explainers
- Call-to-action posts

## Troubleshooting

### Common Issues

**My post doesn't appear:**
- Check that you saved the `blog-posts.json` file
- Verify the JSON syntax is valid (use a JSON validator online)
- Make sure you added the post at the beginning of the array

**Formatting looks wrong:**
- Check for missing `\n\n` between paragraphs
- Verify you escaped quotes properly (`\"`)
- Make sure all commas are in the right places

**JSON syntax errors:**
- Each post except the last needs a comma after its closing `}`
- All strings must be in quotes
- No trailing commas allowed

### Getting Help

If you run into issues:
1. Check the existing posts in `blog-posts.json` for reference
2. Use an online JSON validator to check syntax
3. Ask a team member for help
4. Reference this guide

## File Locations Reference

- **Blog posts data**: `assets/data/blog-posts.json`
- **Template**: `assets/data/blog-post-template.json`
- **Blog page**: `blog.html`
- **This guide**: `HOW-TO-POST-BLOGS.md`

---

*Remember: The blog posts appear in reverse chronological order (newest first), so always add new posts at the beginning of the array.*
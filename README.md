# Hugo live reload broken for Chinese tags

This Hugo site was built following the official [quick start](https://gohugo.io/getting-started/quick-start/).
I added a post that contains both Chinese and English tags.

To reproduce the issue, follow these steps:

1. Run `hugo server`
2. Navigate to `http://localhost:1313/tags/%E6%AC%A2%E8%BF%8E/`
3. You can also open a new tab and visit `http://localhost:1313/tags/eng/` for comparison
4. Edit `content/posts/a-post.md` and change the title or content
5. The Chinese tag page does not reload, while the English tag page reloads as expected

### linked issue
https://github.com/gohugoio/hugo/issues/14240

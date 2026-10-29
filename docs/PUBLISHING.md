# Editing and publishing

This site is built with Hugo Extended. Run `hugo server` to preview locally and `hugo --minify` to build.

## Adding a write-up
1. `hugo new post/my-post.md`
2. Fill in the title, description, categories, and tags, write the content, then set `draft = false`.
3. Optional cover: put an image in `static/posts-cover/` and set `cover = "posts-cover/name.webp"` (otherwise the default scene is used).
4. Push to `main`. GitHub Actions builds, verifies, and deploys it.

## Where things live
- Profile copy: `content/about.md` and `data/about.toml`
- Team and friends: `data/team.toml`, `data/friends.toml`
- Links (GitHub, Telegram, etc.): `hugo.toml`
- Logbook, archives, search, RSS: `content/post/`, `content/archives/`, `content/search.md`
- Starter entry to replace or delete: `content/post/hello-world.md`

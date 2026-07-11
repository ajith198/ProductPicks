# Affiliate configuration

**Status: NO real Amazon Associates tracking ID yet.**

This site does not currently have an approved Amazon Associates account or a real tracking ID. Until a real tracking ID is added below, every affiliate link in every post must use the literal placeholder string:

```
AMAZON_AFFILIATE_LINK_PLACEHOLDER
```

Example of how a link should look in a post while the placeholder is active:

```markdown
[JOOLA Perseus Paddle](https://www.amazon.com/dp/EXAMPLE?tag=AMAZON_AFFILIATE_LINK_PLACEHOLDER)
```

## When the human adds a real tracking ID

Once the site owner has an approved Amazon Associates account, they should replace this section with:

```
Tracking ID: your-real-tag-20
```

**Important process note for future automated runs:** once a real tracking ID is set here, use it in all posts written *after* that point. Do NOT go back and retroactively edit old posts that used the placeholder — leave them as-is.

## Current tracking ID

_(none set — placeholder mode active)_

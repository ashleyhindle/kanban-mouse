# Kanban Mouse

A terminal-based Kanban board using Laravel Prompts, inspired by [Joe Tannenbaum's blog post](https://blog.joe.codes/hacking-laravel-prompts-for-fun-and-profit).

**But** with 100% more mouse support. Whether it's sensible or not.

- Hover
- Drag & drop
- Right click context menu
- Left click 'move card'
- Scroll wheel card selection

## Use locally

```bash
git clone git@github.com:ashleyhindle/kanban-mouse.git
cd kanban-mouse
composer install

php kanban.php
```

# Purpose
This is really just to show how to do it, what's available, and what's possible.

It's not production ready, it's not an app you should use to manage your todos.

It's a demo of what's possible if you ignore your other life commitments.

## Most interesting files
- `app/Themes/Default/KanbanRender.php` but particularly the lines using `getMoveCursorTo()`
    - This shows how we 'overlay' the dragged card, and context menu, on top of the default render
- `app/Mouse.php`
- `app/MouseEvent.php`
- `app/Kanban.php`

# Support & Credits

This was developed by Ashley Hindle. If you like it, please star it, share it, and let me know!

- [Bluesky](https://bsky.app/profile/ashleyhindle.com)
- [Twitter](https://twitter.com/ashleyhindle)
- Website [https://ashleyhindle.com](https://ashleyhindle.com)

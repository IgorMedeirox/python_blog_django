```markdown
# 📰 Django Blog System

Welcome to my fully-featured **Blog Project**, built with 💙 Django!  
This is not just a blog — it's a mini content management system, complete with admin enhancements, rich text editing, image resizing, custom slugs, and a robust category/tag structure. Oh, and it looks good too. 😉

---

## 🧠 Features

- 🔍 SEO-friendly slugs auto-generated with custom logic
- ✍️ Rich text editing using **Django Summernote**
- 🧱 Modular structure: `Posts`, `Pages`, `Categories`, and `Tags`
- 📎 Media handling with image resizing and file attachment logic
- ⚙️ Admin dashboard customized for content editing, filtering, and linking
- 🧠 Smart filtering with class-based views for authors, categories, tags & search

---

## 🚀 Technologies

- 🐍 Python 3
- ⚙️ Django
- 🛠️ Django Admin (with enhanced UX)
- 🎨 Django Summernote for WYSIWYG editing
- 🔧 Custom utilities for slugs and image manipulation

---

## 📂 Main Components

| Model        | Purpose                                 |
|--------------|------------------------------------------|
| `Post`       | Blog post with image, author, category, tags |
| `Page`       | Standalone content (like an About page)     |
| `Category`   | Groups posts under categories               |
| `Tag`        | Hashtag-style tags for posts                |
| `Attachment` | Handles file uploads with resizing          |

---

## 🖥️ Admin Interface Goodies

- Editable status fields like `is_published` directly in list view
- Searchable by ID, slug, title, and more 🔎
- Prepopulated fields for slugs based on titles/names
- Inline access to published links with `mark_safe` 💾
- Pagination, filtering, and autocomplete fields for tags and categories

---

## 🔗 URL Routing

```py
urlpatterns = [
    path('', PostListView.as_view(), name='index'),
    path('post/<slug:slug>/', PostDetailView.as_view(), name='post'),
    path('page/<slug:slug>/', PageDetailView.as_view(), name='page'),
    path('created_by/<int:author_pk>/', CreatedByListView.as_view(), name='created_by'),
    path('category/<slug:slug>/', CategoryListView.as_view(), name='category'),
    path('tag/<slug:slug>/', TagListView.as_view(), name='tag'),
    path('search/', SearchListView.as_view(), name='search'),
]
```

---

## 🌟 Highlights

- ✨ Admin-powered post previews with safe HTML links
- 🧼 Clean and scalable codebase, with reusable managers and utility functions
- 💾 Easy customization for attachments and cover image display
- 🧵 Integrates seamlessly with Django’s user authentication and permissions

---

## 🙋‍♂️ About the Author

I'm a passionate Django developer who loves building projects that are clean, scalable, and fun to maintain.  
This blog was crafted to level up my backend skills — and also happens to be a great place to write ✍️ about tech, life, or pizza.

---

## 📜 License

Open-source and friendly — just like me!  
Use it, fork it, improve it. 🍕

```

If you want, I can help add badges, setup instructions, or visual mockups. Just say the word!
```

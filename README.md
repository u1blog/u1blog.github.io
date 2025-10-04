# u1blog.github.io

This is the Jekyll-powered blog for u1.au.

## Getting Started

To get the project running locally, follow these steps:

1.  **Install dependencies:**

    ```bash
    bundle install
    ```

2.  **Serve the site:**

    ```bash
    bundle exec jekyll serve
    ```

The site will be available at `http://localhost:4000`.

## Creating a New Post

To create a new post, use the `scripts/new` script:

```bash
./scripts/new Your Post Title
```

This will create a new file in the `_posts` directory with the correct filename format and default front matter.

## Adding a New Category

To add a new category, you need to do two things:

1.  **Add the category to a post's front matter.** In the post file, add the category to the `categories` list:

    ```yaml
    ---
    layout: post
    title: "My Awesome Post"
    categories: my-new-category
    ---
    ```

2.  **Create a category page.** In the `categories` directory, create a new file named `my-new-category.html` with the following content:

    ```yaml
    ---
    layout: category
    title: My New Category
    category: my-new-category
    ---
    ```

This will automatically create a new page for the category and add it to the "Categories" dropdown in the navigation.

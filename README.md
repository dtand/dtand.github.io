# Daniel Anderson's Portfolio

A personal portfolio website built with Jekyll and the Minima theme, showcasing my projects and experience.

## Features

- Clean, responsive design using the Minima theme
- Project showcase pages
- Blog support
- Easy to customize and maintain

## Prerequisites

Before you can run this project locally, you'll need:

- **Homebrew** (macOS package manager) - [Install Homebrew](https://brew.sh/)
- **Ruby 2.7+** - Installed via Homebrew
- **Bundler** - Ruby gem management tool

## Installation

### 1. Install Ruby via Homebrew

Since macOS comes with an older system Ruby, install a newer version using Homebrew:

```bash
brew install ruby
```

### 2. Add Homebrew Ruby to your PATH

Add these lines to your `~/.zshrc` file (or run them in your terminal for the current session):

```bash
export PATH="/opt/homebrew/opt/ruby/bin:$PATH"
export PATH="/opt/homebrew/lib/ruby/gems/3.4.0/bin:$PATH"
```

Then reload your shell configuration:

```bash
source ~/.zshrc
```

### 3. Verify Ruby installation

```bash
ruby --version
# Should show Ruby 3.4.x or higher
```

### 4. Install Bundler

```bash
gem install bundler
```

### 5. Install project dependencies

Navigate to the project directory and install the required gems:

```bash
cd portfolio-markdown
bundle install
```

## Running Locally

Start the Jekyll development server:

```bash
bundle exec jekyll serve
```

Your site will be available at [http://127.0.0.1:4000/](http://127.0.0.1:4000/)

The server will automatically rebuild the site when you make changes to files. Press `Ctrl+C` to stop the server.

## Project Structure

```
.
├── _config.yml           # Site configuration
├── _includes/            # Reusable HTML components
├── _layouts/             # Page templates
├── _site/                # Generated site (don't edit)
├── assets/               # CSS, images, and other assets
├── projects/             # Project markdown files
├── about.md              # About page
├── blog.md               # Blog page
├── index.md              # Homepage
└── projects.md           # Projects listing page
```

## Customization

- **Site settings**: Edit `_config.yml` to change the site title, description, and other settings
- **Content**: Markdown files in the root and `projects/` directory
- **Styling**: Custom styles can be added to `assets/main.scss`
- **Layouts**: Modify HTML templates in `_layouts/` and `_includes/`

## Adding New Projects

1. Create a new Markdown file in the `projects/` directory
2. Add front matter with title and other metadata
3. Write your project description in Markdown
4. The project will automatically appear on the projects page

## Deployment Options

This site can be deployed to:

- **GitHub Pages** - Free hosting with automatic builds
- **Netlify** - Free tier with continuous deployment
- **Vercel** - Fast, free hosting with automatic deployments

## Troubleshooting

### Permission Errors with System Ruby

If you get permission errors when installing gems, make sure you're using the Homebrew Ruby (not the system Ruby):

```bash
which ruby
# Should show: /opt/homebrew/opt/ruby/bin/ruby
```

### Port Already in Use

If port 4000 is already in use, specify a different port:

```bash
bundle exec jekyll serve --port 4001
```

### Deprecation Warnings

The Sass deprecation warnings during build are normal and won't affect the site's functionality.

## License

This portfolio is personal property. Feel free to use this as inspiration for your own portfolio.

## Contact

Daniel Anderson

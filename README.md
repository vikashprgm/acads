# ACADS
Static Content Hosting for Juniors

To run this locally,

### Step 1: Install Ruby & Build Tools

Open your terminal and run this to get Ruby and the necessary compilation tools (needed for building Jekyll's dependencies).

```bash
sudo pacman -S ruby base-devel
```

### Step 2: Install Jekyll

Now install the Jekyll and Bundler gems:

```bash
gem install jekyll bundler
```

### Step 3: Run Your Site

Now go to your project folder in VS Code (or terminal) and run the standard commands:

1.  **Install dependencies** (reads your `Gemfile`):

    ```bash
    bundle install
    ```

2.  **Start the server:**

    ```bash
    bundle exec jekyll serve
    ```

You should see `Server address: http://127.0.0.1:4000/`.

### Troubleshooting Tips

If you get an error saying **"webrick not found"** or similar during `bundle install`:

1.  Make sure your `Gemfile` (in the project folder) looks exactly like this:
    ```ruby
    source "https://rubygems.org"

    gem "jekyll"
    gem "webrick"
    ```
2.  Run `bundle update` to refresh everything.

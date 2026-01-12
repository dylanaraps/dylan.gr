# Dylan's website

My simple blog system.


## Dependencies

- [`dpp`](https://github.com/dylanaraps/dpp)
- POSIX `make`
- POSIX `shell`
- POSIX `awk`, `date`, `mkdir`, `rm`, `sed`, `tr`
- `base64`


## Usage

```sh
# Build website.
make

# Create post.
make post

# Start local server.
make serve
```

## Configuration

Edit `./config`.


## Markup

Pretty much just plain text.

- Like markdown, text between blank lines is grouped and enclosed within `<p></p>`.
- Inline links are automatically turned into `<a href="LINK">LINK</a>`.
- `[ALNUM]` not at start of line creates an anchor link `[<a href="#ALNUM">ALNUM</a>]`.
- `[ALNUM]` at start of line creates the destination `[<span id="#ALNUM">ALNUM</span>]`.


## Post Format

```
#tag #tag #tag

Fri, 12 Dec 2025 07:24:15 +0200

TITLE

CONTENT
```


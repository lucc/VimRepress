#Welcome
VimRepress is a plugin for managing wordpress blog from Vim, using Markdown syntax.

This is a repository for Preston's fork.

##Features
 * NEW/EDIT/DELETE wordpress Posts/Pages.
 * In both Markdown / HTML format.
 * Markdown text stored in the custom fields of wordpress.
 * Upload attachments.
 * Insert code highlight section.
 * Preview a posts in local compiled version, or remote draft.
 * wordpress.com account supported.
 * Multiple account supported.

##Commands Reference
 * BlogList     [post|page]
 * BlogNew      [post|page]
 * BlogSave     [publish|draft]
 * BlogPreview  [local|publish|draft]
 * BlogUpload   *[path/to/your/local/file]
 * BlogOpen     *[post id or full article URL]
 * BlogSwitch   [0,1,2 ... N, number of account in your config]
 * BlogCode     [type of lang for the <pre> element]
 
  (Commands with a `*`, argument must be present.)


##CONFIGURE

Edit ~/.vimrc , add a variable named VIMPRESS. Multiple blog configurations are supported.

Example:
{{{
let VIMPRESS = [{'username':'user',
                \'password':'pass',
                \'blog_url':'http://your-first-blog.com/'
                \},
                \{'username':'user',
                \'blog_url':'http://your-second-blog.com/'
                \}]
}}}
Hardcoding the password is optional. If a password is not provided the plugin will prompt for one the first time it's needed.


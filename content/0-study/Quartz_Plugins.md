---
title: Plugins
draft: true
---

# Plugins

May 24, 20261 min read

Quartz’s functionality is provided by a collection of first-party community plugins. Each plugin can be enabled, disabled, and configured via `quartz.config.yaml`. See [Configuration](https://quartz.jzhao.xyz/configuration#plugins) for details on how to manage plugins.

> Internal vs Community Plugins
> 
> Quartz has two kinds of plugins:
> 
> - **Community plugins** are standalone repositories under [`quartz-community`](https://github.com/quartz-community). In TS overrides, they use `ExternalPlugin.X()` (imported from `.quartz/plugins`).
> - **Internal plugins** are built into Quartz core (Assets, Static, ComponentResources, NotFoundPage). In TS overrides, they use `Plugin.X()` (imported from `./quartz/plugins`).

## Plugin types

Quartz plugins fall into several categories:

- **Transformers** process content during the build, e.g. parsing frontmatter, highlighting syntax, or resolving links.
- **Filters** decide which content files to include or exclude from the output.
- **Page Types** generate HTML pages — one per content file, folder, tag, canvas, or bases view.
- **Components** render UI elements in the page layout (sidebars, headers, footers, etc.).

## First-party plugins

All PluginsTransformersFiltersPage TypesEmittersComponents

Showing 44 of 44 entries

|Plugin|Repository|Enabled|Required|Description|
|---|---|---|---|---|
|Category Component17|   |   |   |   |
|[ArticleTitle](https://quartz.jzhao.xyz/plugins/articletitle)|[quartz-community/article-title](https://github.com/quartz-community/article-title)|||Renders the article title as an h1 heading.|
|[Backlinks](https://quartz.jzhao.xyz/plugins/backlinks)|[quartz-community/backlinks](https://github.com/quartz-community/backlinks)|||Shows pages that link to the current page.|
|[Breadcrumbs](https://quartz.jzhao.xyz/plugins/breadcrumbs)|[quartz-community/breadcrumbs](https://github.com/quartz-community/breadcrumbs)|||Breadcrumb navigation trail.|
|[Comments](https://quartz.jzhao.xyz/plugins/comments)|[quartz-community/comments](https://github.com/quartz-community/comments)|||Comment system integration (Giscus, Utterances, etc.).|
|[ContentMeta](https://quartz.jzhao.xyz/plugins/contentmeta)|[quartz-community/content-meta](https://github.com/quartz-community/content-meta)|||Displays creation date and reading time.|
|[Darkmode](https://quartz.jzhao.xyz/plugins/darkmode)|[quartz-community/darkmode](https://github.com/quartz-community/darkmode)|||Toggle between light and dark themes.|
|[Explorer](https://quartz.jzhao.xyz/plugins/explorer)|[quartz-community/explorer](https://github.com/quartz-community/explorer)|||File tree explorer sidebar.|
|[Footer](https://quartz.jzhao.xyz/plugins/footer)|[quartz-community/footer](https://github.com/quartz-community/footer)|||Page footer with configurable links.|
|[Graph](https://quartz.jzhao.xyz/plugins/graph)|[quartz-community/graph](https://github.com/quartz-community/graph)|||Interactive link graph visualization.|
|[NoteProperties](https://quartz.jzhao.xyz/plugins/noteproperties)|[quartz-community/note-properties](https://github.com/quartz-community/note-properties)|||Displays frontmatter properties in a collapsible panel.|
|[PageTitle](https://quartz.jzhao.xyz/plugins/pagetitle)|[quartz-community/page-title](https://github.com/quartz-community/page-title)|||Renders the site title as a home link.|
|[ReaderMode](https://quartz.jzhao.xyz/plugins/readermode)|[quartz-community/reader-mode](https://github.com/quartz-community/reader-mode)|||Distraction-free reading mode toggle.|
|[RecentNotes](https://quartz.jzhao.xyz/plugins/recentnotes)|[quartz-community/recent-notes](https://github.com/quartz-community/recent-notes)|||Displays a list of recently modified notes.|
|[Search](https://quartz.jzhao.xyz/plugins/search)|[quartz-community/search](https://github.com/quartz-community/search)|||Full-text search with tag filtering and keyboard navigation.|
|[Spacer](https://quartz.jzhao.xyz/plugins/spacer)|[quartz-community/spacer](https://github.com/quartz-community/spacer)|||Flexible spacer for layout groups.|
|[StackedPages](https://quartz.jzhao.xyz/plugins/stackedpages)|[quartz-community/stacked-pages](https://github.com/quartz-community/stacked-pages)|||Andy Matuschak-style stacked sliding panes.|
|[TagList](https://quartz.jzhao.xyz/plugins/taglist)|[quartz-community/tag-list](https://github.com/quartz-community/tag-list)|||Renders tags as clickable links.|
|Category Emitter4|   |   |   |   |
|[AliasRedirects](https://quartz.jzhao.xyz/plugins/aliasredirects)|[quartz-community/alias-redirects](https://github.com/quartz-community/alias-redirects)|||Generates redirect pages from frontmatter aliases.|
|[CNAME](https://quartz.jzhao.xyz/plugins/cname)|[quartz-community/cname](https://github.com/quartz-community/cname)|||Emits a CNAME file for custom domain deployment.|
|[ContentIndex](https://quartz.jzhao.xyz/plugins/contentindex)|[quartz-community/content-index](https://github.com/quartz-community/content-index)|||Generates sitemap, RSS feed, and content index.|
|[Favicon](https://quartz.jzhao.xyz/plugins/favicon)|[quartz-community/favicon](https://github.com/quartz-community/favicon)|||Emits the site favicon.|
|Category Filter2|   |   |   |   |
|[ExplicitPublish](https://quartz.jzhao.xyz/plugins/explicitpublish)|[quartz-community/explicit-publish](https://github.com/quartz-community/explicit-publish)|||Only publishes pages explicitly marked with publish: true.|
|[RemoveDrafts](https://quartz.jzhao.xyz/plugins/removedrafts)|[quartz-community/remove-draft](https://github.com/quartz-community/remove-draft)|||Filters out pages marked as drafts.|
|Category Other1|   |   |   |   |
|[Custom OG Images](https://quartz.jzhao.xyz/plugins/customogimages)|[quartz-community/og-image](https://github.com/quartz-community/og-image)|||Generates Open Graph social preview images.|
|Category Page Type5|   |   |   |   |
|[BasesPage](https://quartz.jzhao.xyz/plugins/basespage)|[quartz-community/bases-page](https://github.com/quartz-community/bases-page)|||Renders Obsidian Bases files as database-style views.|
|[CanvasPage](https://quartz.jzhao.xyz/plugins/canvaspage)|[quartz-community/canvas-page](https://github.com/quartz-community/canvas-page)|||Renders JSON Canvas files as interactive, pannable pages.|
|[ContentPage](https://quartz.jzhao.xyz/plugins/contentpage)|[quartz-community/content-page](https://github.com/quartz-community/content-page)|||Generates HTML pages for Markdown content.|
|[FolderPage](https://quartz.jzhao.xyz/plugins/folderpage)|[quartz-community/folder-page](https://github.com/quartz-community/folder-page)|||Generates listing pages for folders.|
|[TagPage](https://quartz.jzhao.xyz/plugins/tagpage)|[quartz-community/tag-page](https://github.com/quartz-community/tag-page)|||Generates listing pages for tags.|
|Category Transformer15|   |   |   |   |
|[Citations](https://quartz.jzhao.xyz/plugins/citations)|[quartz-community/citations](https://github.com/quartz-community/citations)|||Academic citation and bibliography support via BibTeX.|
|[CrawlLinks](https://quartz.jzhao.xyz/plugins/crawllinks)|[quartz-community/crawl-links](https://github.com/quartz-community/crawl-links)|||Parses and resolves internal links. Removing it is not recommended.|
|[CreatedModifiedDate](https://quartz.jzhao.xyz/plugins/createdmodifieddate)|[quartz-community/created-modified-date](https://github.com/quartz-community/created-modified-date)|||Determines creation and modification dates from frontmatter, git, or filesystem.|
|[Description](https://quartz.jzhao.xyz/plugins/description)|[quartz-community/description](https://github.com/quartz-community/description)|||Generates page descriptions for metadata and previews.|
|[EncryptedPages](https://quartz.jzhao.xyz/plugins/encryptedpages)|[quartz-community/encrypted-pages](https://github.com/quartz-community/encrypted-pages)|||Password-protected encrypted pages with shadow content index.|
|[Frontmatter](https://quartz.jzhao.xyz/plugins/frontmatter)|[quartz-community/note-properties](https://github.com/quartz-community/note-properties)|||Parses frontmatter and displays note properties in a collapsible panel.|
|[GitHubFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/githubflavoredmarkdown)|[quartz-community/github-flavored-markdown](https://github.com/quartz-community/github-flavored-markdown)|||GitHub Flavored Markdown support (tables, task lists, footnotes, strikethrough).|
|[HardLineBreaks](https://quartz.jzhao.xyz/plugins/hardlinebreaks)|[quartz-community/hard-line-breaks](https://github.com/quartz-community/hard-line-breaks)|||Treats single newlines as hard line breaks.|
|[Latex](https://quartz.jzhao.xyz/plugins/latex)|[quartz-community/latex](https://github.com/quartz-community/latex)|||Renders LaTeX math expressions via KaTeX or Typst.|
|[ObsidianFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/obsidianflavoredmarkdown)|[quartz-community/obsidian-flavored-markdown](https://github.com/quartz-community/obsidian-flavored-markdown)|||Obsidian-specific Markdown extensions (wikilinks, callouts, highlights, tags, embeds).|
|[OxHugoFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/oxhugoflavoredmarkdown)|[quartz-community/ox-hugo](https://github.com/quartz-community/ox-hugo)|||Compatibility for ox-hugo exported Org-mode files.|
|[RoamFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/roamflavoredmarkdown)|[quartz-community/roam](https://github.com/quartz-community/roam)|||Compatibility for Roam Research export format.|
|[SyntaxHighlighting](https://quartz.jzhao.xyz/plugins/syntaxhighlighting)|[quartz-community/syntax-highlighting](https://github.com/quartz-community/syntax-highlighting)|||Syntax highlighting for code blocks.|
|[TableOfContents](https://quartz.jzhao.xyz/plugins/tableofcontents)|[quartz-community/table-of-contents](https://github.com/quartz-community/table-of-contents)|||Generates and renders a table of contents from headings.|
|[UnlistedPages](https://quartz.jzhao.xyz/plugins/unlistedpages)|[quartz-community/unlisted-pages](https://github.com/quartz-community/unlisted-pages)|||Hides pages from navigation and indexes while still publishing them.|

> Multi-category plugins
> 
> Some plugins span multiple categories. **TableOfContents** is both a transformer and a component. **EncryptedPages** is a transformer, emitter, and component. They appear in each relevant category above.

48 items under this folder.

- May 24, 2026
    
    ### [AliasRedirects](https://quartz.jzhao.xyz/plugins/aliasredirects)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- May 24, 2026
    
    ### [ArticleTitle](https://quartz.jzhao.xyz/plugins/articletitle)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Backlinks](https://quartz.jzhao.xyz/plugins/backlinks)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [BasesPage](https://quartz.jzhao.xyz/plugins/basespage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Breadcrumbs](https://quartz.jzhao.xyz/plugins/breadcrumbs)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [CNAME](https://quartz.jzhao.xyz/plugins/cname)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- May 24, 2026
    
    ### [CanvasPage](https://quartz.jzhao.xyz/plugins/canvaspage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    
- May 24, 2026
    
    ### [Citations](https://quartz.jzhao.xyz/plugins/citations)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [Comments](https://quartz.jzhao.xyz/plugins/comments)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [ContentIndex](https://quartz.jzhao.xyz/plugins/contentindex)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- May 24, 2026
    
    ### [ContentMeta](https://quartz.jzhao.xyz/plugins/contentmeta)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [ContentPage](https://quartz.jzhao.xyz/plugins/contentpage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    
- May 24, 2026
    
    ### [CrawlLinks](https://quartz.jzhao.xyz/plugins/crawllinks)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [CreatedModifiedDate](https://quartz.jzhao.xyz/plugins/createdmodifieddate)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [Custom OG Images](https://quartz.jzhao.xyz/plugins/customogimages)
    
    - [feature/emitter](https://quartz.jzhao.xyz/tags/feature/emitter)
    
- May 24, 2026
    
    ### [Darkmode](https://quartz.jzhao.xyz/plugins/darkmode)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Description](https://quartz.jzhao.xyz/plugins/description)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [EncryptedPages](https://quartz.jzhao.xyz/plugins/encryptedpages)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- May 24, 2026
    
    ### [ExplicitPublish](https://quartz.jzhao.xyz/plugins/explicitpublish)
    
    - [plugin/filter](https://quartz.jzhao.xyz/tags/plugin/filter)
    
- May 24, 2026
    
    ### [Explorer](https://quartz.jzhao.xyz/plugins/explorer)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Favicon](https://quartz.jzhao.xyz/plugins/favicon)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- May 24, 2026
    
    ### [FolderPage](https://quartz.jzhao.xyz/plugins/folderpage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    
- May 24, 2026
    
    ### [Footer](https://quartz.jzhao.xyz/plugins/footer)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Frontmatter](https://quartz.jzhao.xyz/plugins/frontmatter)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [GitHubFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/githubflavoredmarkdown)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [Graph](https://quartz.jzhao.xyz/plugins/graph)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [HardLineBreaks](https://quartz.jzhao.xyz/plugins/hardlinebreaks)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [Latex](https://quartz.jzhao.xyz/plugins/latex)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [NoteProperties](https://quartz.jzhao.xyz/plugins/noteproperties)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [ObsidianFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/obsidianflavoredmarkdown)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [OxHugoFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/oxhugoflavoredmarkdown)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [PageTitle](https://quartz.jzhao.xyz/plugins/pagetitle)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [ReaderMode](https://quartz.jzhao.xyz/plugins/readermode)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [RecentNotes](https://quartz.jzhao.xyz/plugins/recentnotes)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [RemoveDrafts](https://quartz.jzhao.xyz/plugins/removedrafts)
    
    - [plugin/filter](https://quartz.jzhao.xyz/tags/plugin/filter)
    
- May 24, 2026
    
    ### [RoamFlavoredMarkdown](https://quartz.jzhao.xyz/plugins/roamflavoredmarkdown)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [Search](https://quartz.jzhao.xyz/plugins/search)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [Spacer](https://quartz.jzhao.xyz/plugins/spacer)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [StackedPages](https://quartz.jzhao.xyz/plugins/stackedpages)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [SyntaxHighlighting](https://quartz.jzhao.xyz/plugins/syntaxhighlighting)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- May 24, 2026
    
    ### [TableOfContents](https://quartz.jzhao.xyz/plugins/tableofcontents)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [TagList](https://quartz.jzhao.xyz/plugins/taglist)
    
    - [plugin/component](https://quartz.jzhao.xyz/tags/plugin/component)
    
- May 24, 2026
    
    ### [TagPage](https://quartz.jzhao.xyz/plugins/tagpage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    
- May 24, 2026
    
    ### [UnlistedPages](https://quartz.jzhao.xyz/plugins/unlistedpages)
    
    - [plugin/transformer](https://quartz.jzhao.xyz/tags/plugin/transformer)
    
- Mar 19, 2026
    
    ### [Assets](https://quartz.jzhao.xyz/plugins/assets)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- Mar 19, 2026
    
    ### [ComponentResources](https://quartz.jzhao.xyz/plugins/componentresources)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
    
- Mar 19, 2026
    
    ### [NotFoundPage](https://quartz.jzhao.xyz/plugins/notfoundpage)
    
    - [plugin/pagetype](https://quartz.jzhao.xyz/tags/plugin/pagetype)
    
- Mar 19, 2026
    
    ### [Static](https://quartz.jzhao.xyz/plugins/static)
    
    - [plugin/emitter](https://quartz.jzhao.xyz/tags/plugin/emitter)
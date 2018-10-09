CKEditor 5 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Check%20out%20CKEditor%205%20on%20GitHub&url=https%3A%2F%2Fgithub.com%2Fckeditor%2Fckeditor5)
===================================

[![npm version](https://badge.fury.io/js/ckeditor5.svg)](https://www.npmjs.com/package/ckeditor5)

[![Build Status](https://travis-ci.org/ckeditor/ckeditor5.svg?branch=master)](https://travis-ci.org/ckeditor/ckeditor5)
[![BrowserStack Status](https://automate.browserstack.com/automate/badge.svg?badge_key=d3hvenZqQVZERFQ5d09FWXdyT0ozVXhLaVltRFRjTTUyZGpvQWNmWVhUUT0tLUZqNlJ1YWRUd0RvdEVOaEptM1B2Q0E9PQ==--c9d3dee40b9b4471ff3fb516d9ecf8d09292c7e0)](https://automate.browserstack.com/public-build/d3hvenZqQVZERFQ5d09FWXdyT0ozVXhLaVltRFRjTTUyZGpvQWNmWVhUUT0tLUZqNlJ1YWRUd0RvdEVOaEptM1B2Q0E9PQ==--c9d3dee40b9b4471ff3fb516d9ecf8d09292c7e0)
[![Dependency Status](https://img.shields.io/david/ckeditor/ckeditor5.svg)](https://david-dm.org/ckeditor/ckeditor5)
[![devDependency Status](https://img.shields.io/david/dev/ckeditor/ckeditor5.svg)](https://david-dm.org/ckeditor/ckeditor5?type=dev)

[![Join the chat at https://gitter.im/ckeditor/ckeditor5](https://badges.gitter.im/ckeditor/ckeditor5.svg)](https://gitter.im/ckeditor/ckeditor5?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Join newsletter](https://img.shields.io/badge/join-newsletter-00cc99.svg)](http://eepurl.com/c3zRPr)
[![Follow twitter](https://img.shields.io/badge/follow-twitter-00cc99.svg)](https://twitter.com/ckeditor)

A set of ready-to-use rich text editors created with a powerful framework. Made with real-time collaborative editing in mind.

![CKEditor 5 Classic rich text editor build screenshot](https://c.cksource.com/a/1/img/npm/ckeditor%205%20classic%20screeshot.png)

## ⚠ This package does not contain any source code

CKEditor 5 is distributed as [four ready-to-use rich text editor builds](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#available-builds) which you can [install from npm](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/installation.html#npm).

You can also [customize the existing builds](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/development/custom-builds.html) or build your own editors and features by using the [CKEditor 5 Framework](https://ckeditor.com/docs/ckeditor5/latest/framework/guides/overview.html).

## Table of contents

* [Quick start](#quick-start)
   * [CKEditor 5 Builds](#ckeditor-5-builds)
   * [CKEditor 5 Framework](#ckeditor-5-framework)
* [Documentation and FAQ](#documentation-and-faq)
* [Contributing and project organization](#contributing-and-project-organization)
   * [Ideas and discussions](#ideas-and-discussions)
   * [Development](#development)
   * [Reporting issues and feature requests](#reporting-issues-and-feature-requests)
* [Releases](#releases)
* [Packages](#packages)
   * [Core libraries](#core-libraries)
   * [Builds](#builds)
   * [Features](#features)
   * [Editors](#editors)
   * [Themes](#themes)
* [License](#license)

## Quick start

### CKEditor 5 Builds

CKEditor 5 Builds are a set of ready-to-use rich text editors. Every "build" provides a single type of editor with a set of features and a default configuration.

The following CKEditor 5 Builds are currently available:

* [Classic editor](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#classic-editor)
* [Inline editor](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#inline-editor)
* [Balloon editor](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#balloon-editor)
* [Document editor](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#document-editor)

#### Example

Creating an editor using a CKEditor 5 build is very simple and can be described in two steps:

1. Load the desired editor via the `<script>` tag.
2. Call the static `create()` method to create the editor.

In your HTML page add an element that CKEditor should replace:

```html
<textarea name="content" id="editor"></textarea>
```

Load the classic editor build (you can choose between [CDN](https://cdn.ckeditor.com/#ckeditor5), [npm](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/installation.html#npm) and [zip downloads](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/installation.html#zip-download)):

```html
<script src="https://cdn.ckeditor.com/ckeditor5/<version>/classic/ckeditor.js"></script>
```

Call the [`ClassicEditor.create()`](https://ckeditor.com/docs/ckeditor5/latest/api/module_editor-classic_classiceditor-ClassicEditor.html#static-function-create) method:

```html
<script>
    ClassicEditor
        .create( document.querySelector( '#editor' ) )
        .catch( error => {
            console.error( error );
        } );
</script>
```

You’re ready to go!

To find out how to start with other builds check the [Quick start guide in the CKEditor 5 documentation](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/quick-start.html).

### CKEditor 5 Framework

CKEditor 5 Builds allow you to quickly and easily initialize one of the many types of editors in your application. At the same time, CKEditor 5 is also a framework for creating custom-made rich text editing solutions.

To find out how to start building your own editor from scratch go to [CKEditor 5 Framework overview section of CKEditor 5 documentation](https://ckeditor.com/docs/ckeditor5/latest/framework/guides/overview.html).

## Documentation and FAQ

To find out more see the following [CKEditor 5 documentation](https://ckeditor.com/docs/ckeditor5/latest/index.html) sections:

* [API documentation](https://ckeditor.com/docs/ckeditor5/latest/api/index.html)
* [CKEditor 5 Framework documentation](https://ckeditor.com/docs/ckeditor5/latest/framework/index.html)
* [CKEditor 5 Builds documentation](https://ckeditor.com/docs/ckeditor5/latest/builds/index.html)
* [CKEditor 5 Features documentation](https://ckeditor.com/docs/ckeditor5/latest/features/index.html)
* [CKEditor 5 Examples](https://ckeditor.com/docs/ckeditor5/latest/examples/index.html)

The documentation is far from being complete and will be constantly evolving (as will the editor) until it is ready for v1.0.0.

For FAQ please go to the [CKEditor Ecosystem help center](https://support.ckeditor.com/hc/en-us).
For a high-level overview of the project see the [CKEditor Ecosystem website](https://ckeditor.com).

## Contributing and project organization

### Ideas and discussions

The main development repository of CKEditor 5 is located at [https://github.com/ckeditor/ckeditor5](https://github.com/ckeditor/ckeditor5). This is the best place for bringing opinions and contributions. Letting the core team know if they are going in the right or wrong direction is great feedback and will be much appreciated!

### Development

CKEditor 5 is a modular, multi-package, multi-repository project. It consists of several packages that create the editing framework, based on which the feature packages are implemented.

The [ckeditor5](https://github.com/ckeditor/ckeditor5) repository is the place that centralizes the development of CKEditor 5. It bundles different packages into a single place, adding the necessary helper tools for the development workflow, like the builder and the test runner. [Basic information on how to set up the development environment](https://ckeditor.com/docs/ckeditor5/latest/framework/guides/contributing/development-environment.html) can be found in the documentation.

### Reporting issues and feature requests

Each repository handles its issues independently. However, it is recommended to report issues in [this repository](https://github.com/ckeditor/ckeditor5/issues) unless you know to which specific repository the issue belongs.

Read more on the [Support](https://ckeditor.com/docs/ckeditor5/latest/framework/guides/support/getting-support.html) page.

## Releases

See CKEditor 5 release blog posts [on the CKEditor blog](https://ckeditor.com/blog/?category=releases&tags=CKEditor-5).

## Packages

### Core libraries

<table>
<thead>
	<tr>
		<th width="30%">Name</th>
		<th width="15%">Version</th>
		<th width="55%">Description</th>
	</tr>
</thead>
<tbody>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-engine"><code>@ckeditor/ckeditor5-engine</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-engine"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-engine.svg" alt="@ckeditor/ckeditor5-engine npm package badge"></a>
	</td>
	<td>
		The editing engine.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-core"><code>@ckeditor/ckeditor5-core</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-core"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-core.svg" alt="@ckeditor/ckeditor5-core npm package badge"></a>
	</td>
	<td>
		The core editor architecture.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-ui"><code>@ckeditor/ckeditor5-ui</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-ui"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-ui.svg" alt="@ckeditor/ckeditor5-ui npm package badge"></a>
	</td>
	<td>
		The editor UI library.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-utils"><code>@ckeditor/ckeditor5-utils</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-utils"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-utils.svg" alt="@ckeditor/ckeditor5-utils npm package badge"></a>
	</td>
	<td>
		The editor utilities library.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-upload"><code>@ckeditor/ckeditor5-upload</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-upload"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-upload.svg" alt="@ckeditor/ckeditor5-upload npm package badge"></a>
	</td>
	<td>
		The file upload utilities.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-widget"><code>@ckeditor/ckeditor5-widget</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-widget"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-widget.svg" alt="@ckeditor/ckeditor5-widget npm package badge"></a>
	</td>
	<td>
		The widget API.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-cloud-services"><code>@ckeditor/ckeditor5-cloud-services</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-cloud-services"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-cloud-services.svg" alt="@ckeditor/ckeditor5-cloud-services npm package badge"></a>
	</td>
	<td>
		CKEditor 5's Cloud Services integration layer.
	</td>
</tr>

</tbody>
</table>

### Builds

<table>
<thead>
	<tr>
		<th width="30%">Name</th>
		<th width="15%">Version</th>
		<th width="55%">Description</th>
	</tr>
</thead>
<tbody>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-build-classic"><code>@ckeditor/ckeditor5-build-classic</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-build-classic"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-build-classic.svg" alt="@ckeditor/ckeditor5-build-classic npm package badge"></a>
	</td>
	<td>
		The classic editor build.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-build-inline"><code>@ckeditor/ckeditor5-build-inline</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-build-inline"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-build-inline.svg" alt="@ckeditor/ckeditor5-build-inline npm package badge"></a>
	</td>
	<td>
		The inline editor build.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-build-balloon"><code>@ckeditor/ckeditor5-build-balloon</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-build-balloon"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-build-balloon.svg" alt="@ckeditor/ckeditor5-build-balloon npm package badge"></a>
	</td>
	<td>
		The balloon editor (Medium-like) build.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-build-decoupled-document"><code>@ckeditor/ckeditor5-build-decoupled-document</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-build-decoupled-document"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-build-decoupled-document.svg" alt="@ckeditor/ckeditor5-build-decoupled-document npm package badge"></a>
	</td>
	<td>
		The document editor build, featuring the decoupled UI editor implementation.
	</td>
</tr>

</tbody>
</table>

### Features

<table>
<thead>
	<tr>
		<th width="30%">Name</th>
		<th width="15%">Version</th>
		<th width="55%">Description</th>
	</tr>
</thead>
<tbody>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-adapter-ckfinder"><code>@ckeditor/ckeditor5-adapter-ckfinder</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-adapter-ckfinder"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-adapter-ckfinder.svg" alt="@ckeditor/ckeditor5-adapter-ckfinder npm package badge"></a>
	</td>
	<td>
		The <a href="https://ckeditor.com/ckeditor-4/ckfinder/">CKFinder</a> adapter for features which require upload capabilities.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-alignment"><code>@ckeditor/ckeditor5-alignment</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-alignment"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-alignment.svg" alt="@ckeditor/ckeditor5-alignment npm package badge"></a>
	</td>
	<td>
		The text alignment feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-autoformat"><code>@ckeditor/ckeditor5-autoformat</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-autoformat"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-autoformat.svg" alt="@ckeditor/ckeditor5-autoformat npm package badge"></a>
	</td>
	<td>
		The autoformatting feature. Replaces predefined characters with a corresponding format (e.g. <code>**foo**</code> becomes bold <code>&lt;strong&gt;foo&lt;/strong&gt;</code>).
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-autosave"><code>@ckeditor/ckeditor5-autosave</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-autosave"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-autosave.svg" alt="@ckeditor/ckeditor5-autosave npm package badge"></a>
	</td>
	<td>
		The autosave feature. Makes it easy to automatically save the data to the backend.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-basic-styles"><code>@ckeditor/ckeditor5-basic-styles</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-basic-styles"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-basic-styles.svg" alt="@ckeditor/ckeditor5-basic-styles npm package badge"></a>
	</td>
	<td>
		The bold, italic, underline and code features.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-block-quote"><code>@ckeditor/ckeditor5-block-quote</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-block-quote"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-block-quote.svg" alt="@ckeditor/ckeditor5-block-quote npm package badge"></a>
	</td>
	<td>
		The block quote feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-clipboard"><code>@ckeditor/ckeditor5-clipboard</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-clipboard"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-clipboard.svg" alt="@ckeditor/ckeditor5-clipboard npm package badge"></a>
	</td>
	<td>
		The clipboard integration.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-enter"><code>@ckeditor/ckeditor5-enter</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-enter"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-enter.svg" alt="@ckeditor/ckeditor5-enter npm package badge"></a>
	</td>
	<td>
		The <kbd>Enter</kbd> key feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-easy-image"><code>@ckeditor/ckeditor5-easy-image</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-easy-image"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-easy-image.svg" alt="@ckeditor/ckeditor5-easy-image npm package badge"></a>
	</td>
	<td>
		Easy Image with CKEditor Cloud Services feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-font"><code>@ckeditor/ckeditor5-font</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-font"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-font.svg" alt="@ckeditor/ckeditor5-font npm package badge"></a>
	</td>
	<td>
		The font size and font family features.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-heading"><code>@ckeditor/ckeditor5-heading</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-heading"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-heading.svg" alt="@ckeditor/ckeditor5-heading npm package badge"></a>
	</td>
	<td>
		The heading feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-highlight"><code>@ckeditor/ckeditor5-highlight</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-highlight"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-highlight.svg" alt="@ckeditor/ckeditor5-highlight npm package badge"></a>
	</td>
	<td>
		The highlight feature (markers and pens).
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-image"><code>@ckeditor/ckeditor5-image</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-image"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-image.svg" alt="@ckeditor/ckeditor5-image npm package badge"></a>
	</td>
	<td>
		The image feature. Supports image styles and captioning.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-link"><code>@ckeditor/ckeditor5-link</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-link"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-link.svg" alt="@ckeditor/ckeditor5-link npm package badge"></a>
	</td>
	<td>
		The link feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-list"><code>@ckeditor/ckeditor5-list</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-list"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-list.svg" alt="@ckeditor/ckeditor5-list npm package badge"></a>
	</td>
	<td>
		The numbered and bulleted lists feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-markdown-gfm"><code>@ckeditor/ckeditor5-markdown-gfm</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-markdown-gfm"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-markdown-gfm.svg" alt="@ckeditor/ckeditor5-markdown-gfm npm package badge"></a>
	</td>
	<td>
		The GitHub-flavored Markdown data processor.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-media-embed"><code>@ckeditor/ckeditor5-media-embed</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-media-embed"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-media-embed.svg" alt="@ckeditor/ckeditor5-media-embed npm package badge"></a>
	</td>
	<td>
		The media embed feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-paragraph"><code>@ckeditor/ckeditor5-paragraph</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-paragraph"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-paragraph.svg" alt="@ckeditor/ckeditor5-paragraph npm package badge"></a>
	</td>
	<td>
		The paragraph feature.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-table"><code>@ckeditor/ckeditor5-table</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-table"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-table.svg" alt="@ckeditor/ckeditor5-table npm package badge"></a>
	</td>
	<td>
		The table feature. Work in progress.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-typing"><code>@ckeditor/ckeditor5-typing</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-typing"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-typing.svg" alt="@ckeditor/ckeditor5-typing npm package badge"></a>
	</td>
	<td>
		The typing and deleting features.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-undo"><code>@ckeditor/ckeditor5-undo</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-undo"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-undo.svg" alt="@ckeditor/ckeditor5-undo npm package badge"></a>
	</td>
	<td>
		The undo feature.
	</td>
</tr>

</tbody>
</table>

### Editors

<table>
<thead>
	<tr>
		<th width="30%">Name</th>
		<th width="15%">Version</th>
		<th width="55%">Description</th>
	</tr>
</thead>
<tbody>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-editor-classic"><code>@ckeditor/ckeditor5-editor-classic</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-editor-classic"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-editor-classic.svg" alt="@ckeditor/ckeditor5-editor-classic npm package badge"></a>
	</td>
	<td>
		The classic editor implementation.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-editor-inline"><code>@ckeditor/ckeditor5-editor-inline</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-editor-inline"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-editor-inline.svg" alt="@ckeditor/ckeditor5-editor-inline npm package badge"></a>
	</td>
	<td>
		The inline editor implementation.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-editor-balloon"><code>@ckeditor/ckeditor5-editor-balloon</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-editor-balloon"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-editor-balloon.svg" alt="@ckeditor/ckeditor5-editor-balloon npm package badge"></a>
	</td>
	<td>
		The balloon editor (Medium-like) implementation.
	</td>
</tr>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-editor-decoupled"><code>@ckeditor/ckeditor5-editor-decoupled</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-editor-decoupled"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-editor-decoupled.svg" alt="@ckeditor/ckeditor5-editor-decoupled npm package badge"></a>
	</td>
	<td>
		The editor implementation with a decoupled UI.
	</td>
</tr>

</tbody>
</table>

### Themes

<table>
<thead>
	<tr>
		<th width="30%">Name</th>
		<th width="15%">Version</th>
		<th width="55%">Description</th>
	</tr>
</thead>
<tbody>

<tr>
	<td>
		<a href="https://github.com/ckeditor/ckeditor5-theme-lark"><code>@ckeditor/ckeditor5-theme-lark</code></a>
	</td>
	<td>
		<a href="https://www.npmjs.com/package/@ckeditor/ckeditor5-theme-lark"><img src="https://img.shields.io/npm/v/@ckeditor/ckeditor5-theme-lark.svg" alt="@ckeditor/ckeditor5-theme-lark npm package badge"></a>
	</td>
	<td>
		The Lark theme.
	</td>
</tr>

</tbody>
</table>

## License

Licensed under the terms of [GNU General Public License Version 2 or later](http://www.gnu.org/licenses/gpl.html). For full details about the license, please check the LICENSE.md file.

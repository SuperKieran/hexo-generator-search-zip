# hexo-generator-search-zip

[![npm](https://img.shields.io/npm/v/hexo-generator-search-zip.svg)](https://www.npmjs.com/package/hexo-generator-search-zip)
[![npm](https://img.shields.io/npm/dm/hexo-generator-search-zip.svg)](https://www.npmjs.com/package/hexo-generator-search-zip)

Generate zip search data for Hexo 3.0. This plugin is used for generating a search index file, which contains all the neccessary data of your articles that you can use to write a local search engine for your blog.

- [Demo](https://go.kieran.top) - try out the search engine in this site's sidebar.
- [Demo Zip output](https://github.com/SuperKieran/hexo-generator-search-zip/blob/master/output/search.zip)

## Install

``` bash
$ npm install hexo-generator-search-zip --save
```

## Options

You can configure this plugin in your root `_config.yml`.

``` yaml
search:
  path: search.json
  zipPath: search.zip
  versionPath: searchVersion.txt
  field: post
```

- **field** - the search scope you want to search, you can chose:
  * **post** (Default) - will only covers all the posts of your blog.
  * **page** - will only covers all the pages of your blog.
  * **all** - will covers all the posts and pages of your blog.

## FAQ

### What's this plugin supposed to do? 

This plugin is used for generating a zip file from your Hexo blog that provides data for searching.

### Where's this file saved to?

After executing `hexo g` you will get the generated result at your public folder.


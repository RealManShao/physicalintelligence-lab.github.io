


# Maintanance of the group website
## Installation
1. Install [Hugo Extended](https://github.com/gohugoio/hugo/releases?page=3). (This repo was tested with hugo [v0.123.8](https://github.com/gohugoio/hugo/releases/tag/v0.123.8))
2. Install Go ``sudo  snap  install  --classic  go``
3. Install Node.js ``sudo  snap  install  --classic  node``
## Structure of the website repo
Most of the change can be conducted by modifying the files in the ``content`` folder. And the related media like pics should be stored in the ``/asset/media`` folder . 
```
.
├── LICENSE.md
├── README.md
├── assets
│   ├── jsconfig.json
│   ├── media
│   └── scss
├── config
│   └── _default
├── content
│   ├── _index.md
│   ├── admin
│   ├── authors
│   ├── contact
│   ├── event
│   ├── people
│   ├── post
│   ├── publication
│   └── tour
├── go.mod
├── go.sum
├── images
│   ├── screenshot.png
│   └── tn.png
├── netlify.toml
├── preview.png
├── static
│   └── uploads
└── theme.toml
```
## How to modify the personal profile
You can commit changes to your profiles by modifying the files in the folder ``/content/authors/<first_name>_<last_name>``.
## Locally preview
Execute following the commands under the website project root path  
1. ``hugo``
2. ``hugo server``
	There will appear a URL for preview.
## Update the changes to the online website
Committing and pushing the modifications to remote repo, the website will update autonoumously by Github Action. 
## Template source and official doc
1. [Template employed](https://hugoblox.com/templates/details/research-group/)
1. [Official doc](https://docs.hugoblox.com/zh-cn/getting-started/install-hugo/)
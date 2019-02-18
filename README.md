**Table of Contents**
* [md_TOC_generator](#md_toc_generator)
* [Intro](#intro)
  * [How it works](#how-it-works)
* [Manual](#manual)
  * [Download Repo](#download-repo)
    * [Copy scripts to /usr/bin](#copy-scripts-to-/usr/bin)
    * [Example](#example)

# md_TOC_generator
Markdown Table of Contents generator

# Intro
Some ruby and shell code to generate Table of Contents for your Markdown document.
The original version of the ruby code is available here [generate_toc.rb](https://gist.github.com/albertodebortoli/9310424)
> (Author [albertodebortoli](https://gist.github.com/albertodebortoli))

## How it works
* Script search *md file
  * For each md file found, the script check if a TOC is already generated
  * Generate TOC using generate_toc_rb script
  * Check if TOC can be generated for this md file
    * Copy TOC in the md file
* Finaly you have to add/commit/push your nice MD file to your repo ;) 
> you can use this script for lazy poeple [gacp script](https://github.com/shitana/git_tools)

# Manual
## Download Repo
```shell
git clone git@github.com:shitana/md_TOC_generator.git
``` 

### Copy scripts to /usr/bin
```shell
cd md_TOC_generator
sudo cp generate_toc* /usr/bin/
``` 

### Example
```shell
generate_toc /home/shitana
  Generate TOC in progress for /home/shitana/github/md_TOC_generator/README.md
  TOC already exists for /home/shitana/github/git_tools/README.md

```

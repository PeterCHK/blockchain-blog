# Blockchain FAQ Blog

[![Build Status](https://travis-ci.org/hexojs/hexo.svg?branch=master)](https://travis-ci.org/hexojs/hexo)  [![NPM version](https://badge.fury.io/js/hexo.svg)](http://badge.fury.io/js/hexo) [![Coverage Status](https://coveralls.io/repos/hexojs/hexo/badge.svg?branch=master)](https://coveralls.io/r/hexojs/hexo?branch=master) [![Build status](https://ci.appveyor.com/api/projects/status/hpx3lduqjj2t6uqq/branch/master?svg=true)](https://ci.appveyor.com/project/tommy351/hexo/branch/master) [![Gitter](https://badges.gitter.im/hexojs/hexo.svg)](https://gitter.im/hexojs/hexo?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Discord Chat](https://img.shields.io/badge/chat-on%20discord-7289da.svg)](https://discord.gg/teM2Anj)
[![dependencies Status](https://david-dm.org/hexojs/hexo/status.svg)](https://david-dm.org/hexojs/hexo) [![devDependencies Status](https://david-dm.org/hexojs/hexo/dev-status.svg)](https://david-dm.org/hexojs/hexo?type=dev)

A fast, simple & powerful blog framework, powered by [Node.js](http://nodejs.org).
Originally forked from hexo.

## Heroku Installation
``` bash
#node, npm and git are prerequisite
$ sudo apt install snapd
$ sudo snap install heroku --classic
```


## Hexo installation

``` bash
$ npm install hexo-cli -g
```

## Quick Start

**Login with Heroku credentials**
``` bash
$ heroku login
#enter heroku email and password
```
**Setup new heroku app**
``` bash
heroku create -a <app-name>
```

**Setup your blog**

``` bash
#this project already initiated
$ hexo init blog

$ cd blog
#change directory before running this to install
npm install hexo-deployer-heroku --save
```

**Start the server**

``` bash
#no need to start local server if push directly to heroku
$ hexo server
```

**Create a new post**

``` bash
$ hexo new "Hello World!"
```


**Clean previous public and database folder**
``` bash
$ hexo clean
```

**Generate static files**
``` bash
#generate new public and database folder for deployment
$ hexo generate
```

**Add heroku git**
``` bash
#peter-blockchain
heroku git:remote -a <git repo name>
```
**Add text @ blog > config.yml**
``` bash
deploy:
  type: heroku
  repo: <repo from heroku>
```

**Deploy static files**
``` bash
$ hexo deploy
```

**Check the heroku website**
``` bash
$ heroku open
```


## More Information

- Visit the [peter-blockchain](peter-blockchain.herokuapp.com) website
- Read the [hexo documentation](https://hexo.io/)
- Find hexo solutions in [troubleshooting](https://hexo.io/docs/troubleshooting.html)
- See the [hexo plugin list](https://hexo.io/plugins/) and the [theme list](https://hexo.io/themes/) on wiki
- Find git repo in [Heroku dashboard](https://dashboard.heroku.com/apps)
- Also check out [Getting Started on Heroku with Node.js](https://devcenter.heroku.com/articles/getting-started-with-nodejs) for getting started on Heroku with Node.js

## License

MIT

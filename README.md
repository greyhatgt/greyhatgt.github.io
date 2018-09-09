# greyhatgt.github.io
Georgia Tech's cyber security student organization, website created with [Hexo](https://hexo.io/)

*this is a note to self*
- deploy to [greyhat.gatech.edu](http://greyhat.gatech.edu) by uploading index.html to [hosting.gatech.edu](https://hosting.gatech.edu/)
- deploy to GitHub sites:
```shell
# prerequisites: npm

# installation
$ npm install hexo-cli -g
$ cd /path/to/greyhatgt.github.io/  # NOT the GitHub.com repo!
$ npm install

# usage
# deployment one-liner
$ hexo clean && hexo generate && cp README.md public/ && cp index.html public/ && hexo deploy
```

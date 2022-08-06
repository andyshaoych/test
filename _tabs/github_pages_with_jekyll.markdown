---
title: pages
icon: fas fa-info-circle
order: 4
---
# Creating a GitHub Pages site with Jekyll  
  https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll  

## create new repo on `github`  
- `andyshaoych.github.io`   

- `git clone` the repo  
  git clone https://github.com/andyshaoych/andyshaoych.github.io.git  

## Install `Jekyll` & `jekyll new site`  
- Install `Jekyll`  
  `gem install bundler jekyll`  

- jekyll new site  
  ```bash
  cd andyshaoych.github.io/  
  jekyll new --skip-bundle .  
  ```
- Update .gitignore with `.DS_Store`  
  .DS_Store  

- comment out `gem "jekyll"` in `Gemfile`    
  `# gem "jekyll", "~> 4.2.2"`   

- uncomment `gem "github-pages"` in `Gemfile`  
  `gem "github-pages", group: :jekyll_plugins`  

- run `bundle install`  
  ```
    $ bundle install
      Fetching gem metadata from https://rubygems.org/...........
      Resolving dependencies.......
      ...
  ```

- start the server locally   
  ```
    $ bundle exec jekyll serve  
      ...
      Server address: http://127.0.0.1:4000/
      Server running... press ctrl-c to stop.
  ```

- Verify the Jekyll site locally   
  ![](images/2022-08-03-00-35-45.png)  

  ![](images/2022-08-03-00-36-38.png)  

## push the code and verify Github Pages site  
- push the code  
  ```
    $ git commit -m "initial site"  
    $ git push  
  ```

- Verify `https://andyshaoych.github.io/`  
  Wait for 30 seconds and view:  
  ![](./images/2022-08-03-00-50-28.png)  


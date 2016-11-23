# Docker Drupal Static Check


## Use with Gitlab-CI

Create file .gitlab-ci.yml
```
image: olragon/drupal-static-check
stages:
  - test
CoderTest:
  stage: test
  script:
    - phpcs --standard=Drupal --extensions=php,module,inc,install,test,profile,theme,css,info,txt,md ./
```

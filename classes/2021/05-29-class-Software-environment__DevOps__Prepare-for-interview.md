# Class 2021-05-29

* conventional commit
  * 
* 共筆軟體介紹： HackMD
  * 建議大家註冊帳號
* QA
  * Test plans
    * example: User Management, Authentication, Authorization, etc.
  * Test cases
    * log in
      * happy path: input correct email, password
      * should not be empty
      * duplicate username
    * log out
    * forget password
    * sign up
  * Test Report
    * totol: 200 cases
    * success: 200
    * failure: 0
* Testing
  * Unit Testing (Dev)
  * Integration Testing (Dev)
  * E2E Testing (Dev, QA)
  * Manual Testing (QA)
  * Smoke Test
* Local Development experience
  * IDE
    * Syntax checking
    * auto fix/format linting on save
    * auto run specific unit test on save
  * commit
    * lint: convetional commit
  * before push -> run full unit test (by using git hook)
* CI/CD
  * Pipeline flow
  * CI: Continuous Integration
    * Linting 
      * code (not auto fix)
      * commit message
    * Static Analysis
    * Testing
      * Unit Testing (Dev)
      * Integration Testing (Dev)
      * Smoke Test
    * Build
  * CD: Continuous Delivery
    * Automate Deployment
      * Code
      * database migration
      * update server config
      * restart/reload services
* DRY principle
  * Do repeat yourself
* How to prepare for an interview
  * 提高被面試的機率
  * Blog
  * Notes
  * Twitter
  * github (TODO: Kos tries to find good github accounts of candidate)
    * fork open source project and modify
      * automation for setting up a new environment
        * os
        * docker
        * tools
        * configs
          * git config
    * side projects
    * website
      * tech
        * client side -> github
        * backend -> cloud (GCP, AWS, Digital Ocean, Linode)
      * content
        * self introduction
        * work experience
          * projects
        * personal projects
        * tools
          * linux
          * languages: php, javascript, golang
          * Unit Test: php unit, jest
          * docker
          * CI/CD: CircleCI
          * Cloud Services: GCP
          * IDE: VS Code
    * Blog
    * open source proejcts
* Github
  * Gist
    * https://gist.github.com/koshuang/87b18953766da787f2ffce1387d82565
* Kent C. Dodds
  * https://kentcdodds.com/blog/how-i-am-so-productive

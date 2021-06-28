# Class2021-06-26

Subject: [Teaching] Laravel & Web Development

## Agenda

- [Deploy and Host a Static Webpage for Free with Netlify](https://egghead.io/lessons/html-5-deploy-and-host-a-static-webpage-for-free-with-netlify)

- 選取的小技巧

  - 如何快速在網頁上選取一段字？

- [外國人才不會說「RD」！工程師最常念錯的 8 個英文字](https://www.businessweekly.com.tw/careers/blog/10419)
- [台灣工程師常唸錯的英文單字
  ](https://blog.privism.org/2012/06/blog-post.html)

- Laravel

  - Route

    - Q: Can we use self-defined prefix other than "api/"?
    - A: Yes, and we can make changes in app/Providers/RouterServiceProvider

    ```php
    protected function mapXRoutes()
    {
      Route:prefix('prefix-name')
          ->namespace('$this->namespace')
          ->group(base_path('routes/router-file-name'));
    }
    ```

  - Static Method
    - ::
    - "New" keyword is not needed when creating instance of static class
  - Custom Service Provider
    - Add ViewServiceProvider

- 驗證 Port 有沒有開啟

  - `netstat -nap |grep 3306`

- SQL Command

  - To show database: `show databases;`
  - To select database to use: `use [database name];`
  - To show data table: `show tables;`

- Docker

  - 列出所有的 container
    - `docker ps`
    - `docker ps -a`
  - 在 container 執行 Command
    - `docker exec -it [command you want]` \*it = interactive
      - `docker exec -it echo hi`
  - 在特定的 container 執行 Command
    - `docker exec -it container-name [command you want]`
    - `docker exec -it container-name php artisan migrate`

- Git
  - Get global ignore file path: `git config --global core.excludesFile`
  - create a file `~/gitignore_global`

```ignore
*.ignore*
*.ignore*/

.vscode/
.ide/
```

- VS Code

  - Plugins
    - `PHP Sort Imports`: auto sort the imports on save.

- HTTP

  - Methods: get, post, update, put, patch, delete, options

- PHP Auto Formatting
  - PHP_CodeSniffer (PHPCS)
  - Articles
    - <https://www.twilio.com/blog/improving-php-code-quality-php-codesniffer-phpcs-laravel>
  - 理想方法 (越快得到回饋越好)
    - IDE 支援
    - Watch Code changes, and then alert
    - git hook: 使用 `pre-commit` hook 去執行 phpcs 驗證那些有被更動的檔案
    - CI: 使用 CI 去執行 phpcs 驗證那些有被更動的檔案
  - 只要有 CI 去卡 Deploy 流程，再加上 Slack/Microsoft Teams 通知

## Homework

- Watch VS Code part of https://www.youtube.com/watch?v=376vZ1wNYPA&t=2787s

## References

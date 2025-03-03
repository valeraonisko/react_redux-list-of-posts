# React + Redux list of posts

## Task

By requesting [https://jsonplaceholder.typicode.com/posts](https://jsonplaceholder.typicode.com/posts), [https://jsonplaceholder.typicode.com/users](), and [https://jsonplaceholder.typicode.com/comments](https://jsonplaceholder.typicode.com/users), create and display a list of posts with the following data on each:

1) the title of the post;
2) the text (body) of the post;
3) the name, email, and address of the author of the post;
4) sublist of the post comments, including the name and email of the author of each comment as well as the comment itself.

Create and use the following components:
- `PostList`,
- `PostListHandler` (Redux container for `PostList`),
- `Post`,
- `PostHandler` (Redux container for `Post`),
- `User`,
- `CommentList`,
- `Comment`,
- `CommentHandler` (Redux container for `Comment`).

You can use the `User` component from both `Post` (with address) and `Comment` (without providing any address). 

There should also be a working "Remove" button alongside every post and every comment on the page.

Initially `PostList` has to present the user with a button labeled "Load". When the user hits the button, the script starts to download the data; the label of the button has to change to "Loading..." and the button must become disabled. Once the data has been loaded, hide the button altogether and display the posts instead.

Additionally, you should provide a capability of filtering the items by text entered by the user (when filtering, you can consider only the title and the text of the post).

## Workflow

- Fork the repository with task
- Clone forked repository 
    ```bash
    git clone git@github.com:<user_name>>/<task_repository>.git
    ```
- Run `npm install` to install dependencies.
- Then develop

## Development mode 

- Run `npm run start` to start `http-server` on `http://localhost:3000`
    When you run server the command line window will no longer be available for 
    writing commands until you stop server (`ctrl + c`). All other commands you 
    need to run in new command line window.
- Follow [HTML, CSS styleguide](https://mate-academy.github.io/style-guides/htmlcss.html)
- Follow [the simplified JS styleguide](https://mate-academy.github.io/style-guides/javascript-standard-modified)
- When you finished `Deploy on gh-pages`

## Deploy on gh-pages

- Build the project
  ```bash
  $ npm run build
  ```
- Commit and push all recent changes
  ```bash
  $ git add .
  $ git commit -m 'commit message'
  $ git push origin master
  ```
- Execute `npm run deploy`. This command will push the `/build` folder to branch
  `gh-pages` in your remote repository. 
- Add links to your demo in readme.md.
  - `[DEMO LINK](https://<your_account>.github.io/<repo_name>/)` - this will be a 
  link to your index.html
- Commit and push all recent changes again.
- Create `Pull Request` from forked repo `(<branch_name>)` to original repo 
(`master`).
- Add a link at `PR` to Google Spreadsheets.

## Project structure

- `src/` - directory for css, js, image, fonts files
- `build/` - directory for built pages

You should be writing code in `src/` directory.

### Demo link

Add link here: `[DEMO LINK](https://<your_account>.github.io/<repo_name>/)`

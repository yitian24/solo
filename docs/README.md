## Personal Docs

### 部署方式

- 创建仓库

  ```bash
  git init xxx
  git clone https://github.com/yitian24/docs.git new-docs
  cd new-docs
  git remote remove origin
  git remote add origin https://github.com/你的用户名/xxx.git
  ```

- 安装依赖
  ```bash
  npm install
  ```

- 正式部署

> ```bash
> # 更新主分支main
> git add .
> git commit -m "update&fix"
> git push -u origin main
> 
> # 部署修改后的文档
> npm run build
> npm run deploy
> ```

- Github pages

  在仓库setting中设置以下选项：

  > Branch: gh-pages
  > Folder: /(root)

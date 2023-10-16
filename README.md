<!--
 * @Author: sheri sheri_situ@163.com
 * @Date: 2023-10-16 15:55:21
 * @LastEditors: sheri sheri_situ@163.com
 * @LastEditTime: 2023-10-16 16:36:18
 * @FilePath: /docusaurus-blog/README.md
-->
Docusaurus是Facebook开源的文档搭建网站，国内国外众多的开源项目均使用了Docusaurus，文档使用 Markdown 编写并可部署在 GitHub Pages 上。
是一款静态站点生成器。释放了 React 的全部潜能，搭建了这款带有快速的客户端导航且交互性极佳的单页应用。即开即用的文档功能不仅仅局限于文档本身，还可用于创建任何类型的网站（个人网站、产品网站、博客、营销着陆页等）。
Docusaurus 设计之初就极度重视开发者及贡献者的体验。

- 使用 React 打造
- 使用 React 扩展与自定义
- 提供您自己的 React 组件，完全掌控网站的浏览体验
- 可扩展
- 使用基础模板搭建网站，随后使用进阶功能及插件
- 开放您的插件源码，与社群共享
- 开发者体验
- 立即撰写您的软件文档
- 统一配置文件可被轻松维护
- 更改后飞速增量编译并热加载
- 基于路由的代码及数据拆分
- 轻松发布至 GitHub Pages、Netlify、Vercel 及其他部署服务

其目标为——快速让用户找到需要的内容，并更好地了解您的产品。我们将与您分享我们的最佳实践，帮助您正确构建自己的文档网站。

## 1、安装
使用命令行工具可以帮助你快速简单地安装 Docusaurus 并搭建网站框架。 你可以在空仓库或现有仓库的任何地方运行这个命令，它会创建一个包含模板文件的新目录
```shell
npx create-docusaurus@latest my-website classic
```
这是一个包含classic经典模板内容的生成命令, 转到你的目录运行。
```shell
cd my-website
npm run start
```
## 2、上传到GitHub
新建git仓库
```shell
git init
git add .
git commit -m "init"
git remote add origin https://github.com/SheriSzeto/docusaurus-blog
git push -f origin master
```
## 3、Vercel 是知名的前端部署和托管平台，这里我们用它来自动部署代码
vercel还自带cdn加速，在速度上比使用通过github pages托管，通过xxx.github.io/xxx访问的速度快，除此以外，还可以自定义域名，可以使用我们自己的域名。
进入Vercel官网，注册账号登录。
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-1.png)
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-2.png)
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-3.png)
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-4.png)
然后点击deploy部署
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-5.png)
当看到这个页面就表示部署成功了。
添加自己的域名部署，打开settings，左侧边栏找到domains，将自己的域名添加进去。
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-6.png)
xxx.vercel.app是Vercel提供的可以直接打开的网站访问地址，如果是要部署到自己的域名上，则需要将这个地址添加到个人域名的解析下，均指向CNAME的解析记录，下面以百度云示例：
![image.png](https://cdn.jsdelivr.net/gh//SheriSzeto/image@main/docusaurus-7.png)


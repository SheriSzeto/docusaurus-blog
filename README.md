<!--
 * @Author: sheri sheri_situ@163.com
 * @Date: 2023-10-16 15:55:21
 * @LastEditors: sheri sheri_situ@163.com
 * @LastEditTime: 2023-10-16 15:55:21
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
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755029088-e9ed396b-fedf-4f55-b25b-9833cf4986c7.png#averageHue=%23020101&clientId=ucbe5924a-9c92-4&from=paste&height=401&id=u5aaee061&originHeight=801&originWidth=1626&originalType=binary&ratio=2&rotation=0&showTitle=false&size=80095&status=done&style=none&taskId=u69ed62db-f7da-4bce-a56c-6e50bf8e2c0&title=&width=813)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755035818-80e25825-d1ca-4d5a-b359-12bb09f253ba.png#averageHue=%230c0b0b&clientId=ucbe5924a-9c92-4&from=paste&height=435&id=u37834a40&originHeight=870&originWidth=1464&originalType=binary&ratio=2&rotation=0&showTitle=false&size=144514&status=done&style=none&taskId=uc2422e71-1a55-4440-a7d0-60a896bfb9d&title=&width=732)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755043393-38820e38-39fe-49aa-8bf2-6c9b4226bbcc.png#averageHue=%23b1846e&clientId=ucbe5924a-9c92-4&from=paste&height=416&id=u26d32b7d&originHeight=831&originWidth=1918&originalType=binary&ratio=2&rotation=0&showTitle=false&size=265103&status=done&style=none&taskId=ud9ae6af8-0132-4bfe-ae7e-4292d9a76f1&title=&width=959)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755235937-18148d80-646e-4942-b535-e1114807381a.png#averageHue=%230a0909&clientId=ucbe5924a-9c92-4&from=paste&height=663&id=u1902d2d4&originHeight=1326&originWidth=2718&originalType=binary&ratio=2&rotation=0&showTitle=false&size=289906&status=done&style=none&taskId=u8ddbddac-0abf-4763-b97b-25b1b63200c&title=&width=1359)
然后点击deploy部署
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755300598-d8c19cc8-e4c6-4324-b929-2009dc661ab3.png#averageHue=%23111010&clientId=ucbe5924a-9c92-4&from=paste&height=616&id=u0c0db003&originHeight=1232&originWidth=2618&originalType=binary&ratio=2&rotation=0&showTitle=false&size=260803&status=done&style=none&taskId=ube7c54ad-e50f-4470-936a-7241f61ef0b&title=&width=1309)
当看到这个页面就表示部署成功了。
添加自己的域名部署，打开settings，左侧边栏找到domains，将自己的域名添加进去。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755423608-0fc38d8b-673d-489a-8719-70094f69023d.png#averageHue=%23040404&clientId=ucbe5924a-9c92-4&from=paste&height=674&id=u91393cd5&originHeight=1348&originWidth=2716&originalType=binary&ratio=2&rotation=0&showTitle=false&size=232915&status=done&style=none&taskId=u88621768-e840-4cb0-82db-488e1729f96&title=&width=1358)
xxx.vercel.app是Vercel提供的可以直接打开的网站访问地址，如果是要部署到自己的域名上，则需要将这个地址添加到个人域名的解析下，均指向CNAME的解析记录，下面以百度云示例：
![image.png](https://cdn.nlark.com/yuque/0/2023/png/21382958/1692755698785-6891931c-8743-4eac-8bb6-63d743155619.png#averageHue=%23f47b6c&clientId=ucbe5924a-9c92-4&from=paste&height=267&id=u50469b65&originHeight=534&originWidth=1917&originalType=binary&ratio=2&rotation=0&showTitle=false&size=80991&status=done&style=none&taskId=u76946212-430a-489c-844b-fc438a11619&title=&width=958.5)

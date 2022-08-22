# kamiro-draw-page
基于 [draw-page-structureVue](https://github.com/famanoder/dps) 的骨架屏方案测试项目。

其实现过程是事先生成待加载的页面骨架，再插入到vue根节点中，待首屏加载完毕，根节点会被替换掉。

这边仅仅是简单的演示一下它的使用方式，后续再进一步研究。

---

#### 启动测试
一键安装依赖并启动
```bash
npm run dev
```
调试的时候，需要把浏览器的网络降速为3g这样，效果会明显一点。

---

#### 自己踩的坑
npm 源一定要设置好，如果使用公司的镜像源的话，记得切换回npm原先的镜像源，不然 dps 一直失效。

**默认 npm 镜像源切换**
```bash
npm cache clean --force
npm config set registry http://registry.npmjs.org
npm config set registry https://registry.npm.taobao.org/
npm install
```

---
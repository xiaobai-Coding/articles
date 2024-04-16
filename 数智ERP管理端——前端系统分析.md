## 变更记录
> 记录每次修订的内容，方便追溯。


## 项目背景
> 对本次项目的背景以及目标进行描述，方便开发者理解需求，对齐上下文。

知识库基础能力的升级，解决以下问题：

- 目录与文档管理分布在不同的页面，用户无法区分两者区别。
- 目录拖拽体验不够流畅，交互细节体验不佳。
### 相关资料
> PRD、设计稿等相关资料，可以通过插入“语雀内容”卡片快速引入关联的语雀文档
> 也可以通过“本地文件”、“附件”上传其他资料。


### 参与人
| **项目负责人** | ... |
| --- | --- |
| **产品经理** | ... |
| **设计师** | ... |
| **工程师** | ... |

## 技术栈
vue3+element-plus+vite+tailwindcss
> tailwindcss文档：[https://tailwindcss.cn](https://tailwindcss.cn)

## 功能模块
ERP管理端属于企云舰的一个子系统，前端分模块进行开发
![](https://cdn.nlark.com/yuque/0/2024/jpeg/36013995/1704789400590-b4ce4df9-0d95-4eeb-8e24-2b669a7637ed.jpeg)
一共有12个大的模块
可以复用的页面有：
财务管理：

- [x] 客户付款凭证
- [x] 到账凭证

业务订单：

- [x] 查看客户资料
- [x] 订单详情

     客户管理：

- [x] 客户详情

    业务员管理/咨询师管理

- [x]  列表
- [x]  详情
- [x] 统计

---

全局统一复用的页面有：

- [x] 列表显示项设置
- [x] 列表导出
- [x] 列表打印

**列表的封装，以保证样式的统一**
![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1704785002891-ce468f88-be67-4231-ae55-c44ebc17b891.png#averageHue=%23fcfbfb&clientId=u1651cf37-0fbf-4&from=paste&height=746&id=usdQn&originHeight=746&originWidth=1241&originalType=binary&ratio=1&rotation=0&showTitle=false&size=81601&status=done&style=none&taskId=u0fd7d3d4-ca88-4d9b-a4f7-b1f3004c16a&title=&width=1241)
展示列表可以封装为一个插槽

1. 列表title
2. 查询条件
3. 按钮组
4. 列表展示

**详情页的封装，以保证样式的统一减少重复工作**
![image.png](https://cdn.nlark.com/yuque/0/2024/png/36013995/1704793474317-9286face-0c32-47d3-bf9d-6e377a53e304.png#averageHue=%23f7f7f6&clientId=u8c6e98a4-4c12-4&from=paste&height=820&id=u58f3cc2b&originHeight=820&originWidth=1264&originalType=binary&ratio=1&rotation=0&showTitle=false&size=75731&status=done&style=none&taskId=u88833b5d-3371-45af-b301-ee2fedf0c78&title=&width=1264)
封装为一个插槽
1.面包屑导航
2.页面title
3.内容区域
## 项目目录
```markdown
### 项目目录
erp
├─ pages                
│  │  ├─ agency-fee   代理费管理          
│  │  ├─ grant         代理费发放   
│  │  │  ├─ detail     详情   
│  │  │  │  └─ index.js   
│  │  │  ├─ js         逻辑部分  
│  │  │  │  ├─ detail.js  
│  │  │  │  └─ list.js    
│  │  │  └─ index.vue  列表   
│  │  └─ statistics            
│  ├─ business-order  业务订单管理
│  ├─ components      公共的组建  
│  ├─ consultant      咨询师管理  
│  ├─ contract        网签管理 
│  ├─ customer        客户管理  
│  ├─ database        资料库  
│  ├─ finance         财务管理 
│  ├─ institution     机构管理  
│  ├─ oa-approve      OA审批
│  ├─ product         产品管理  
│  ├─ salesman        业务员管理  
│  └─ table-operations 表格操作  
├─ support              
│  ├─ assets            
│  │  ├─ icon  字体图标         
│  │  ├─ img   图片         
│  │  └─ style 样式         
│  └─ utils   工具类          
└─ README.md         

```



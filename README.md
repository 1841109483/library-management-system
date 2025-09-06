# 图书管理系统2026届最新

#### 介绍
library-management-system
图书管理系统2026届最新 需要帮助私 MrN1579

# 图书管理系统

这是一个完整的图书管理系统，包含前端Vue.js应用和后端Django REST框架API。系统支持图书管理、分类管理、借阅管理和用户管理等功能。

最近无聊直播的时候写的，分享出来给同学们学习下

## 项目结构

项目由两个主要部分组成：

- `my-vue-project/`: 基于Vue.js的前端应用
- `myproject/`: 基于Django的后端API

## 后端 (Django)

### 技术栈

- Python 3.x
- Django 5.2
- Django REST Framework
- MySQL
- JWT认证

### 应用模块

- `books`: 图书管理模块
- `categories`: 图书分类管理
- `users`: 用户管理和认证
- `media`: 媒体文件存储(如图书封面)

### 数据库配置

系统使用MySQL数据库，配置如下：

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'books_db_manage',
        'USER': 'root',
        'PASSWORD': '123456',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### API端点

- `/api/books/`: 图书管理
- `/api/categories/`: 分类管理
- `/api/borrows/`: 借阅管理
- `/api/users/`: 用户管理
- `/api/token/`: JWT令牌获取
- `/api/token/refresh/`: JWT令牌刷新

## 前端 (Vue.js)

### 技术栈

- Vue.js 3.2
- Vue Router 4.0
- Axios
- CSS3

### 主要组件

- `Admin.vue`: 管理员界面，包含图书、分类、借阅和用户管理
- `Login.vue`: 用户登录
- `Register.vue`: 用户注册
- `BookList.vue`: 图书列表展示
- `UserCenter.vue`: 用户中心
- `MyBorrows.vue`: 我的借阅
- 各种表单组件: `BookForm.vue`, `CategoryForm.vue`, `UserForm.vue`, `BorrowingForm.vue`

### 功能特性

1. **图书管理**
   - 图书列表展示
   - 新增/编辑/删除图书
   - 图书搜索
   - 图书分类筛选

2. **分类管理**
   - 分类列表展示
   - 新增/编辑/删除分类
   - 分类层级管理

3. **借阅管理**
   - 借阅图书
   - 归还图书
   - 借阅历史查看
   - 逾期提醒

4. **用户管理**
   - 用户注册/登录
   - 用户信息管理
   - 权限控制(管理员/普通用户)

## 运行项目

### 后端启动

1. 确保已安装Python和MySQL
2. 创建并激活虚拟环境(可选)
3. 安装依赖:（我好像没输出这个，没关系了，缺什么包就装什么包吧）
   ```
   pip install -r requirements.txt
   ```
4. 创建数据库:
   ```
   CREATE DATABASE books_db_manage CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
   ```
5. 迁移数据库:
   ```
   python manage.py migrate
   ```
6. 创建超级用户:
   ```
   python manage.py createsuperuser
   ```
7. 启动服务器:
   ```
   python manage.py runserver
   ```

### 前端启动

1. 确保已安装Node.js和npm
2. 安装依赖:
   ```
   cd my-vue-project
   npm install
   ```
3. 启动开发服务器:
   ```
   npm run serve
   ```
4. 构建生产版本:（可以不需要输入）
   ```
   npm run build
   ```

## 系统截图（我也不知道重复不，具体去看看仓库里面的照片就行，已经停全面的了，这里可以忽略）



![1](https://github.com/user-attachments/assets/af04ade3-7850-4534-baac-f1344710c9ce)



## 开发者

- MrN1579

## 许可证

本项目采用MIT许可证。详见LICENSE文件。 

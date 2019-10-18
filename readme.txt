https://github.com/typicode/json-server
新建一个文件夹jsonServer
vscode进入该文件夹

安装：
npm install json-server --save

生成package.json
npm init --yes

修改执行命令：
"scripts": {
    "json:server": "json-server --watch db.json"
}

本地新建db.json
填写json数据格式的数据
{
    "users": [
        {
            "name": "张三",
            "phone": "11-11-11",
            "email": "zhangsan@gmail.com",
            "id": 1,
            "age": 30,
            "companyId": 1
        },
        {
            "name": "李四",
            "phone": "22-22-22",
            "email": "lisi@gmail.com",
            "id": 2,
            "age": 29,
            "companyId": 2
        },
        {
            "name": "王二",
            "phone": "33-33-33",
            "email": "wangeer@gmail.com",
            "id": 3,
            "age": 32,
            "companyId": 3
        },
        {
            "name": "王二er",
            "phone": "44-44-44",
            "email": "wangeer@gmail.com",
            "id": 4,
            "age": 32,
            "companyId": 3
        }
    ],

    "companies": [
        {
            "id": 1,
            "name": "Apple",
            "des": "apple is good"
        },
        {
            "id": 2,
            "name": "organ",
            "des": "organ is good"
        },
        {
            "id": 3,
            "name": "haha",
            "des": "haha is good"
        }
    ]
}


启动项目：
npm run json:server
即可打开地址查看数据
http://localhost:3000/users
http://localhost:3000/companies



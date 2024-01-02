# python-learn
# 学习fastapi
# 第一天 
## 创建环境
    python3 -m venv venv  
    source venv/bin/activate
## 安装
    pip install fastapi_amis_admin 
    ```
    from fastapi import FastAPI
    app = FastAPI()
    
    @app.get("/")
    async def root():
        return {"Hello": "World"}
    if __name__ == '__main__':
        uvicorn.run(app="main:app", host="127.0.0.1", port=8080, reload=True, debug=True)
    ```
    参数	作用
    app	运行的 py 文件:FastAPI 实例对象
    host	访问url，默认 127.0.0.1
    port	访问端口，默认 8080
    reload	热更新，有内容修改自动重启服务器
    debug	同 reload
    reload_dirs	设置需要 reload 的目录，List[str] 类型
    log_level	设置日志级别，默认 info
## uvicorn运行方式
    https://blog.csdn.net/weixin_46248273/article/details/120284287?spm=1001.2101.3001.6650.2&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-2-120284287-blog-123818140.235%5Ev40%5Epc_relevant_3m_sort_dl_base2&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7ERate-2-120284287-blog-123818140.235%5Ev40%5Epc_relevant_3m_sort_dl_base2&utm_relevant_index=5

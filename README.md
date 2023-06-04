# alist-replit
 部署
【部署教程】(https://www.bilibili.com/video/BV1pV4y197Eb/?spm_id_from=333.788.recommend_more_video.1&vd_source=997338a3c326e04408c3f23ee16b63ac)
## Database
You may need to use another remote MySQL/Postgres database as local sqlite3 is public for everyone. Some Free MySQL/Postgres Databases:

- https://db4free.net/
- https://remotemysql.com/
- https://www.freesqldatabase.com/
- https://planetscale.com/
- https://bit.io/
- https://www.elephantsql.com/
- https://scalingo.com/
- http://cloud.yugabyte.com/
- 监控防休眠https://uptimerobot.com/
How to change the database?
> Switch to `secrets` tab then edit `System environment variables`.You can also edit raw json:
> ```json
> {
>   "DB_TYPE":"mysql",
>   "DB_HOST":"sql.com",
>   "DB_PORT":"3306",
>   "DB_USER":"alist",
>   "DB_PASS":"password",
>   "DB_NAME":"alist",
>   "DB_TABLE_PREFIX":"alist_",
>   "DB_SSL_MODE":"true"
> }
> ```
> The secrets is private so you don't need to worry about leaking your data.

### Sample Config https://bit.io/
> ```json
> {
>   "DB_TYPE": "postgres",
>   "DB_HOST": "db.bit.io",
>   "DB_PORT": "5432",
>   "DB_USER": "user",
>   "DB_PASS": "password",
>   "DB_NAME": "user/alist",
>   "DB_TABLE_PREFIX": "alist_",
>   "DB_SSL_MODE": "require"
> }
> ```
##更新alist  
备份已部署好的（下载项目文件），之后全部上传之后点击下载(https://github.com/alist-org/alist/releases/latest/download/alist-linux-musl-amd64.tar.gz)
两次解压后改文件名替换备份文件中的

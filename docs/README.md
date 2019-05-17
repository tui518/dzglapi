#一、接口url
>1、测试环境：http://test-jcyy.aierp.cn:8089/jinan/jrzt
2、demo环境：https://es-demo.jchl.com/jinan/jrzt
3、生产环境：https://es.jchl.com/jinan/jrzt

#二、参数说明：参数是拼接在url的形式

```
  username:登陆账号
  pwd：密码
  nsrsbh：纳税人识别号
  khmc：客户名称
  ssh： u6Ccx22usn80DcVnPgFBUSCC7OuR4olq/1DyHSAKMyLm7A/MSEprHdBgELiv2I/0（认证字符串） 
```

#三、调用方式：GET请求
##3.1 测试环境示例
>http://test-jcyy.aierp.cn:8089/jinan/jrzt?username=15650148229&pwd=Admin1&nsrsbh=123123FFF123123123DD&khmc=刘七花&ssh=u6Ccx22usn80DcVnPgFBUSCC7OuR4olq/1DyHSAKMyLm7A/MSEprHdBgELiv2I/0

##3.2 demo环境示例
>https://es-demo.jchl.com/jinan/jrzt?username=15650148229&pwd=Admin1&nsrsbh=12345678901234567&khmc=XXXX&ssh=u6Ccx22usn80DcVnPgFBUSCC7OuR4olq/1DyHSAKMyLm7A/MSEprHdBgELiv2I/0

##3.3 生产环境示例
>https://es.jchl.com/jinan/jrzt？username=15650148229&pwd=Admin1&nsrsbh=123123FFF123123123DD&khmc=刘七花&ssh=u6Ccx22usn80DcVnPgFBUSCC7OuR4olq/1DyHSAKMyLm7A/MSEprHdBgELiv2I/0

#四、返回值说明
```
{
    "code": "1", （1为成功 0为失败）
    "url": "http://debug-dz.aierp.cn:8089/index.html?appkey=10001007&code=72b64641e7fb892561015b07a6d6d866&orgId=6024559123208192&orgName=%E5%88%98%E4%B8%83%E8%8A%B1"
}
```

>**注意事项**
4.1失败会返回具体原因；
4.2建议传账号和密码时传管理员的账号和密码，密码为明文格式；
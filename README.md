# Railway-Ngrok

利用Ngrok将Railway docker内网穿透做vps使用

## 一、注册 Railway 账号和 Ngrok 账号

1、点击 [Railway](https://railway.app/login) 进入网站注册 Railway 账号，直接使用  github 账号登录即可

2、点击 [Ngrok](https://dashboard.ngrok.com/auth) 进入网站，点击下方的 `Sign up for free!` 注册账号

3、再次进入 [Ngrok](https://dashboard.ngrok.com/auth) 复制保存你的 `Authtoken`

ps: Ngrok 的免费账号一个地区只能拥有一个隧道服务，所以想要部署多个项目请修改地区

## 二、部署

点击下方按钮部署

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/AkashiCoin/Railway-Ngrok&envs=NGROK_TOKEN,PORT,REGION&NGROK_TOKENDesc=在Ngrok注册得到的Authtoken&PORTDesc=你需要的开放的端口，默认80&PORTDefault=80&REGIONDesc=Ngrok的地区，默认jp，可选us/eu/ap/au/sa/jp/in&REGIONDefault=jp&referralCode=IGBnmG)

`NGROK_TOKEN` 中填入在 `Ngrok` 注册得到的 `Authtoken`

`PORT` 中填入你搭建应用的端口，Railway 会自动将其转发到给你的域名上

`REGION` 中填入隧道所在的地区，距离越近越好

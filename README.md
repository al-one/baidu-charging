# 🔌 百度充电站

<a name="install"></a>
## 安装/更新

> 以下几种方法任选其一！

#### 方法1: [HACS (**点击这里安装**)](https://my.home-assistant.io/redirect/hacs_repository/?owner=hasscc&repository=baidu-charging&category=integration)

#### 方法2: 通过 Samba / SFTP 手动安装
> [下载](https://github.com/hasscc/baidu-charging/archive/main.zip)解压并复制`custom_components/baidu_charging`文件夹到HA配置目录下的`custom_components`文件夹

#### 方法3: 通过`SSH`或`Terminal & SSH`加载项执行一键安装命令
```shell
wget -O - https://get.hacs.vip | DOMAIN=baidu_charging REPO_PATH=hasscc/baidu-charging ARCHIVE_TAG=main bash -
```

#### 方法4: `shell_command`服务
1. 复制代码到HA配置文件 `configuration.yaml`
    ```yaml
    shell_command:
      update_baidu_charging: |-
        wget -O - https://get.hacs.vip | DOMAIN=baidu_charging REPO_PATH=hasscc/baidu-charging ARCHIVE_TAG=main bash -
    ```
2. 重启HA使配置生效
3. 在开发者工具中执行服务 [`service: shell_command.update_baidu_charging`](https://my.home-assistant.io/redirect/developer_call_service/?service=shell_command.update_baidu_charging)
4. 再次重启HA使插件生效


<a name="config"></a>
## 配置

> [⚙️ 配置](https://my.home-assistant.io/redirect/config) > 设备与服务 > [🧩 集成](https://my.home-assistant.io/redirect/integrations) > [➕ 添加集成](https://my.home-assistant.io/redirect/config_flow_start?domain=baidu_charging) > 🔍 搜索 [`百度充电站`](https://my.home-assistant.io/redirect/config_flow_start?domain=baidu_charging)

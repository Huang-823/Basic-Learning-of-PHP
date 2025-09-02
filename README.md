# <center> PHP基础学习</center>  

## 一.PHP相关知识了解  

### 1.PHP 定义  

一种 ==服务器端== 的HTML ==脚本/编程语言== ,是一种简单的、面向对象的、解释影的、健壮的、安全的、性能非常之高的、独立于架构的、可移植的、动杰的脚本语言。是一种广泛用于 0pen souzce(开放源代码)的尤其还合 web开发并可以嵌入HTML的多用设脚本语言。它的语法接近c，Java和 Per1，而且容易学习。该语言让 ob 开发人员快速的书写 ==动态生成的网页==。  

### 2.静态网站与动态网站  

**1）静态网站**  

1. 网页内容一经发布到网站服务器上，无论是否有用户访问，每个静态网页的内容都是保存在网站服务器上的，也就是说，静态网页是实实在在保存在服务器上的件，每个网页都是一个独立的文件;
2. 静态网页的内容相对稳定，因此 ==容易被搜索引整检索==;
3. ==静态网页没有数据库的支持==，在网站制作和维护方面工作量较大，因此当网站信息量很大时完全依壹静态网页制作方式比较困难;
4. 静态网页的==交互性较差==，在功能方面有较大的限制。  

**2）动态网站**  

1. 交互性: ==网页会根据用户的要求和选择而动态地改变和响应==，浏览器作为客户端，成为一个动态交流的桥梁，动态网页的交互性也是今后Wed发展的潮流。
2. 自动更新:即无须手动更新HTML文档，便会自动生成新页面，可以大大节省工作量。
3. 因时因人而变:即当不同时间、不同用户访问同一网址时会出现不同页面。
4. 此外动态网页是与静态网页相对应的，也就是说，网页的后不是`.htm`、`.html`、`.shtml`、`.xml`等静志网页的常见形式,而是以`.asp`、`.jsp`、`.php`、`.perl`、`.cgi`等形式为后缀。在动态网页网址中有一个标志性的符号--“?””

## 3.IP的概念  

IP(Internet Protocol)，网络之间互联协议。网络之间互连的协议也就是为 ==计算机网络相互连接进行通信而设计的协议==，在因特网中，它是能使连接到网上的所有计算机网络实现相互通信的一套规则，规定了计算机在因特网上进行通信时应当遵守的规则。任何厂家生产的计算机系统，只要遵守IP协议就可以与因特网互连互通。==IP 地址具有唯一性==。(每台电脑都有一个唯一的 IP地址)。  

### 4.域名  

域名(Domain Name)，是由一串用点分隔的名字组成(www,itcast.cn)的 Internet上某一台计算机或计算机组的名称，用于在数据传输时标识计算机的电子方位(有时也指地理位置，地理上的域名，指代有行政自主权的一个地方区域)。城名是一个IP地址上有“面具”。一个域名的目的是便于记忆和沟通的一组服务器的地址(网站，电子邮件，FTP 等)。域名作为力所能及难忘的互联网参与者的名称。  

### 5.DNS  

DNS(Domain Name System，域名系统)，因特网上作为域名和 IP 地址相互映射的一个分布式数据库,能够使用户更方便的访问互联网，而不用去记住能够被机器直接读取的 IP数串。通过主机名,最终得到该主机名对应的 IP 地址的过程叫做域名解析( 或主机名解析)。  

### 6.端口  

端口(Port)，可以认为是设备与外界通讯交流的出口。口可分为==虚拟端口==和==物理端口==，其中虚拟端口指计算机内部或交换机路由器内的端口，不可见。例如计算机中的 80端口、21 端口、23 端口等。物理端口又称为接口，是可见端口，计算机背板的 RJ45 网口，交换机路由器集线器等 RJ45 端口。  

```用户输入域名localhost:端口-->DNS(localhost 127.0.0.1)-->服务器电脑-->软件(服务)```  

### 二.Web程序的访问流程  

Web 分为两类:静态网站和动态网站  

*浏览器发起访问-->DNS 解析域名-->服务器电脑-->服务软件*  
**1）静态网站访问：**
[![pVcZLuD.md.png](https://s21.ax1x.com/2025/08/30/pVcZLuD.md.png)](https://imgse.com/i/pVcZLuD)  
**2）动态网站访问：**  
动态网站访问流程与静态差不多，但是会多出几个内容:服务器端解析、数据库
[![pVcZvEd.md.png](https://s21.ax1x.com/2025/08/30/pVcZvEd.md.png)](https://imgse.com/i/pVcZvEd)  

## 三.Httpd.exe应用  

### 1.服务器进程:运行之后才能够工作  

[![pVgV08P.md.png](https://s21.ax1x.com/2025/09/02/pVgV08P.md.png)](https://imgse.com/i/pVgV08P)  

### 2.用来查看 Apache 具有哪些功能以及配置文件是否有错：httpd或者 httpd.exe(文件所在目录)  

[![pVgVsKS.png](https://s21.ax1x.com/2025/09/02/pVgVsKS.png)](https://imgse.com/i/pVgVsKS)  

### 3.查看使用的模块：httpd -M  

[![pVgVDv8.png](https://s21.ax1x.com/2025/09/02/pVgVDv8.png)](https://imgse.com/i/pVgVDv8)  

### 4.验证配置文件是否有效：httpd-t  

[![pVgKNVS.md.png](https://s21.ax1x.com/2025/09/02/pVgKNVS.md.png)](https://imgse.com/i/pVgKNVS)  

## 四.配置默认站点  

### 1.让 Apache 确定服务器上访问的位置:网站文件夹所在位置  

**Httpd.conf:DocumentRoot**  
[![pVgKLIe.md.png](https://s21.ax1x.com/2025/09/02/pVgKLIe.md.png)](https://imgse.com/i/pVgKLIe)

### 2.方便用户使用名字访问对应的网站:给文件夹对应的取一个别名  

**Httpd.conf:ServerName**  
[![pVgKbVO.md.png](https://s21.ax1x.com/2025/09/02/pVgKbVO.md.png)](https://imgse.com/i/pVgKbVO)

**端口可以单独实现：httpd.conf:listen**  
[![pVgKqaD.md.png](https://s21.ax1x.com/2025/09/02/pVgKqaD.md.png)](https://imgse.com/i/pVgKqaD)  

### ==3.凡是涉及到Apache配置文件的修改，那么需要重启Apache才能生效==  

### 4.实现 DNS 域名解析:通常默认站点都是本地 DNS:hosts 文件  

[![pVgMpsP.md.png](https://s21.ax1x.com/2025/09/02/pVgMpsP.md.png)](https://imgse.com/i/pVgMpsP)  

## 五.安装php语言  

### 1.获取php安装文件（[官网]）  

### 2.解压缩  

### 3.安装：将压缩包放到与Apache相同目录下，重命名php  

## 六.Php.exe的应用  

### PHP.exe 就是可以解析 PHP 代码转变成 HTML 代码从而让浏览器可以解析的

#### 1.通过 CMD 控制器进入到 php.exe 所在目录.

` `

#### 2。通过 php.exe 运行命令来指定要解析的 PHP脚本就可以:php.exe -f PHP 文件所在路态  

` `

## 七.配置Apache加载PHP 模块  

### 1.Apache 加载 PHP 模块:在 Apache 的主配置文件中加载对应的 PHP 提供的模块 LoadModule php5_module PHP 所提供的模块链接所在路径  

` `

### 2.Apache 分配工作给 PHP 模块:如果是 PHP 代码就交给 PHP 处理:文件后缀判断.php 结尾肯定是 PHP 代码  

`AddType application/x-httpd-php .php`  

` `  

### 3、 将 PHP 的配置文件加载到 Apache 配置文件中:共同生效。

#### 3.1 在 Apache 中指定 PHP 配置文件所在路径。

` `

#### 3.2 php.ini文件默认是不存在的，是以 developient 和 production 格式存在，需要格式化

` `


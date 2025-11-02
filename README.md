# 前言

大家好，本次分享的是基于Spring Boot的医药管理系统毕业设计项目。本项目是适用于Java计算机毕业设计的一个实战项目，涉及前后端的开发、数据库设计等多个方面。以下将详细介绍本项目的相关内容。

# 内容介绍

本项目主要实现了医药管理的基本功能，包括药品信息管理、库存管理、销售管理、用户管理等模块。通过使用Spring Boot框架，结合MySQL数据库，构建了一个易于维护、扩展性强的医药管理系统。同时，前端采用了JS、Vue、CSS3等技术，使得系统界面简洁、响应速度快。

# 技术介绍

## 语言：Java
## 使用框架：Spring Boot
## 前端技术：JS、Vue、CSS3
## 开发工具：IDEA/Eclipse
## 数据库：MySQL 5.7/8.0
## 数据库管理工具：phpstudy/Navicat
## JDK版本：jdk1.8
## Maven: apache-maven 3.8.1-bin
## 前端环境：Node.Js 12\14\16

# 核心代码

以下为药品信息管理模块的部分核心代码：

```java
@RestController
@RequestMapping("/drug")
public class DrugController {

    @Autowired
    private DrugService drugService;

    @PostMapping("/add")
    public ResponseEntity<String> addDrug(@RequestBody Drug drug) {
        try {
            drugService.addDrug(drug);
            return new ResponseEntity<>("添加成功", HttpStatus.OK);
        } catch (Exception e) {
            return new ResponseEntity<>(e.getMessage(), HttpStatus.INTERNAL_SERVER_ERROR);
        }
    }

    @GetMapping("/list")
    public ResponseEntity<List<Drug>> listDrugs() {
        return new ResponseEntity<>(drugService.listDrugs(), HttpStatus.OK);
    }
}
```

# 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/306626/22/26386/141203/689dd3c2F287b43e2/3629f3f1aee323d2.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/309216/23/26667/85973/689dd3a2F63f3b5f4/ac33464a4124b682.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/318158/18/23560/80264/689dd3a3F88f8c58f/ff689c4a2c97fcac.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/311607/4/24084/81031/689dd3a4Febb78222/5e717302a03a85c5.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/308625/7/26775/82009/689dd3a4Fc321044b/32945c885ac9c005.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/306592/4/26637/53177/689dd3a5Fea77efdc/917c6be7d4f3d950.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/328220/28/4518/27740/689dd3a6Fd5790e8b/024723267166d8f5.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/294850/31/22711/40665/689dd3a6Fdbb80343/d3d9172818e5b9a8.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/312050/23/26414/38089/689dd3a7Fdff7871e/3fa2433e18575089.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/309285/21/26609/41782/689dd3a7F9a9681c2/8c3404f727a15638.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)

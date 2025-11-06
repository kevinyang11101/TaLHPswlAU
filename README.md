# 前言

大家好，这是一个基于Spring Boot的医院信息管理系统。这个项目是我的毕业设计，经过一段时间的努力，现在将其开源分享给大家。在此，感谢所有支持和帮助过我的人。

# 内容介绍

这个医院信息管理系统主要包括以下功能模块：挂号管理、医生管理、病人管理、药品管理、就诊管理等。通过这个系统，可以实现医院各科室、医生、病人等信息的实时更新和查询，为医院提供高效、便捷的信息化管理手段。本项目后端采用Java语言开发，前端采用Vue框架，前后端分离的设计模式，易于维护和扩展。

# 技术介绍

## 语言：Java
## 使用框架：Spring Boot
## 前端技术：JS、Vue、css3
## 开发工具：IDEA/Eclipse
## 数据库：MySQL 5.7/8.0
## 数据库管理工具：phpstudy/Navicat
## JDK版本：jdk1.8
## Maven: apache-maven 3.8.1-bin
## 前端环境：Node.Js 12\14\16

# 核心代码

以下是一段关于医生管理的核心代码示例：

```java
@RestController
@RequestMapping("/api/doctor")
public class DoctorController {

    @Autowired
    private DoctorService doctorService;

    // 查询所有医生信息
    @GetMapping("/list")
    public ResponseEntity<List<Doctor>> list() {
        List<Doctor> doctors = doctorService.list();
        return ResponseEntity.ok(doctors);
    }

    // 添加医生信息
    @PostMapping("/add")
    public ResponseEntity<Void> add(@RequestBody Doctor doctor) {
        doctorService.add(doctor);
        return ResponseEntity.ok().build();
    }

    // 更新医生信息
    @PutMapping("/update")
    public ResponseEntity<Void> update(@RequestBody Doctor doctor) {
        doctorService.update(doctor);
        return ResponseEntity.ok().build();
    }

    // 删除医生信息
    @DeleteMapping("/delete/{id}")
    public ResponseEntity<Void> delete(@PathVariable("id") Long id) {
        doctorService.delete(id);
        return ResponseEntity.ok().build();
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

![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/289781/13/19151/103043/689ee503F4d53456b/37c7906784b93232.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/325662/25/4934/36769/689ee4dcF52fa163a/140818600e7188f7.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/323949/3/4799/26397/689ee4dcFaf590e37/9053d38b22c4d14f.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/311534/19/26437/34616/689ee4deF29a2f895/2b995ee59d5bc276.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/323756/25/4721/44636/689ee4dfFd17565dd/f7970372d0c75617.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/327911/26/4819/36715/689ee4dfFab946690/b2a7dc897b19e8e6.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/296052/35/9375/46760/689ee4e0F3f909ee4/3c993f54e708452e.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/309412/37/26701/22928/689ee4e1Fd5b6fb01/7ce9fe1fd42693de.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/307058/23/26790/39399/689ee4e2Fe27d569a/938002da592588cc.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/324380/7/4857/26635/689ee4e2F0c3284a7/4742d97cb961b9df.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)

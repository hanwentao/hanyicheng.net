---
title: 首页
date: 2022-05-20T11:54:29+08:00
---

# 韩意铖的个人主页 {#header}

我是

* []{#grade}的[]{#type}学生
* 狂热的汽车爱好者（距离我能拿驾照还有 []{#days} 天）
* **仿真车**资深收藏家
  * [Tomica 多美卡](https://www.tomy.cn/tomica)
  * [Matchbox 火柴盒](https://www.matchbox.com/)
  * [Hot Wheels 风火轮](https://www.hotwheels.com/)
* [乐高](https://www.lego.com/zh-cn)小玩家（[我和爸爸的收藏](https://brickver.com/@hanwentao)）
* [赛车总动员](https://cars.disney.com/)的忠实粉丝
* 钢琴练习者
* 班级足球队队员
* 灵魂画家

**声明**：目前主页由[我爸](https://hanwentao.net)开发维护。

![韩意铖](hanyicheng.jpg)\

<script>
  const GRADE = ["一年级", "二年级", "三年级", "四年级", "五年级", "六年级",
                 "初一", "初二", "初三", "高一", "高二", "高三",
                 "大一", "大二", "大三", "大四"];
  const TYPE = "小小小小小小中中中中中中大大大大";

  function computeAge(year, month, day) {
    let now = new Date();
    let thisYear = now.getFullYear();
    let age = thisYear - year;
    let birthday = new Date(thisYear, month - 1, day);
    return now >= birthday ? age : age - 1;
  }

  let target = Date.parse("2033-07-17T00:00:00+08:00");
  let now = Date.now();
  let days = Math.floor((target - now) / (24 * 60 * 60 * 1000));
  let grade = computeAge(2021, 9, 1);
  document.getElementById("grade").innerText = GRADE[grade];
  document.getElementById("type").innerText = TYPE[grade];
  document.getElementById("days").innerText = days;
</script>

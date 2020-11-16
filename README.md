# 平安复旦自动打卡

使用GitHub Actions实现全自动打卡。

## 如何使用
1. Fork本代码库
2. 配置Secret  
   在 Settings - Secret 页面添加如下内容
   - USERNAME: 学号
   - PASSWORD: UIS密码
   - PUSH_KEY[可选]: Server酱SCKEY，用于推送通知，详见http://sc.ftqq.com/
3. 修改[work.yml](./.github/workflow/work.yml)中的`schedule`为你喜欢的打卡时间

## 说明
打卡时使用前一日地理位置信息，如位置变更请提前停止自动打卡，到新位置手动打卡一次再开启。  
未经充分测试，不保证最终效果，请酌情使用。

# 营销系统接口对接规范

[参见wiki](https://github.com/qiaofangyun/qf-marketing-openApi/wiki)

## 目录
* 对接准备
    * [分配授权秘钥](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/分配授权秘钥)
* 签名方式
    * [签名方式](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/签名方式)

* 登录营销系统
    * [获取登录营销系统的URL](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/获取登录营销系统的URL)
    * [获取采房相关Url](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/获取采房相关Url)

* 营销系统-SAAS专用-组织机构
    * [同步公司](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/同步公司)
    * [同步员工](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/同步员工)
    * [营销系统变更公司对应的商户信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/v10%E6%95%B0%E6%8D%AE%E8%BF%81%E7%A7%BB%E5%88%B0v20%E9%80%9A%E7%9F%A5%E8%90%A5%E9%94%80%E7%B3%BB%E7%BB%9F%E5%8F%98%E6%9B%B4%E5%95%86%E6%88%B7%E4%BF%A1%E6%81%AF)

* 营销系统-搜索接口-组织机构
   * [根据营销内部员工uuids获取员工信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据营销内部员工uuids获取员工信息)
   * [根据营销内部公司uuids获取公司信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据营销内部公司uuids获取公司信息)

* 公共营销房-SAAS专用-二手房
    * [同步房源到营销库(v10/v20/vip)（不推荐使用）](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量同步房源)
    * [同步房源到营销库(v10/v20/vip)(包含新增字段)](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量同步房源(包含新增字段))
    * [批量同步房源图片信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量同步房源图片信息)
    * [同步全景房vr图片信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/同步全景房vr图片信息)
    * [同步房源视频信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量同步房源视频信息)
* 公共营销房-搜索接口-二手房
    * [根据外部公司uuid等搜索公共营销库](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/搜索公共营销库房源)
    * [根据营销房源内部uuids查询公共营销库房源](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据uuids查询公共营销库房源)
    * [根据营销内部公司uuid和房源源编号查询公共营销库房源uuids](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据营销内部公司uuid和房源源编号查询公共营销库房源uuids)

    * [根据营销内部公司uuid和房源外部uuid查询公司营销库全景房vr图片信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据公司uuid和房源uuid查询全景房vr图片信息
)
    * [根据营销内部公司uuid和房源外部uuid查询公司营销库房源视频信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据公司uuid和房源uuid查询房源视频信息)

* 公共营销房-SAAS专用-营销工具
     * [根据房源外部uuid获取营销工具模块列表](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E8%8E%B7%E5%8F%96%E8%90%A5%E9%94%80%E5%B7%A5%E5%85%B7%E6%A8%A1%E5%9D%97%E5%88%97%E8%A1%A8%E6%8E%A5%E5%8F%A3)

* 公共营销房-SAAS专用-新房
    * [同步新房楼盘基础信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E6%89%B9%E9%87%8F%E5%90%8C%E6%AD%A5%E6%96%B0%E6%88%BF%E6%A5%BC%E7%9B%98%E5%9F%BA%E7%A1%80%E4%BF%A1%E6%81%AF)
    * [同步新房楼盘户型信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E6%89%B9%E9%87%8F%E5%90%8C%E6%AD%A5%E6%96%B0%E6%88%BF%E6%A5%BC%E7%9B%98%E6%88%B7%E5%9E%8B%E4%BF%A1%E6%81%AF)
    * [同步新房楼盘图片信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E6%89%B9%E9%87%8F%E5%90%8C%E6%AD%A5%E6%96%B0%E6%88%BF%E6%A5%BC%E7%9B%98%E5%9B%BE%E7%89%87(%E7%9B%B8%E5%86%8C)%E4%BF%A1%E6%81%AF)

* 公共营销房-搜索接口-新房
    * [搜索公共营销库新房楼盘](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/搜索公共营销库新房楼盘)
    * [根据新房楼盘uuids查询公共营销库新房楼盘](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据新房楼盘uuids查询公共营销库新房楼盘)
    * [根据新房楼盘uuids查询公共营销库新房楼盘](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据新房楼盘uuids查询新房楼盘户型信息)
    * [根据新房楼盘uuids查询新房楼盘图片信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/根据新房楼盘uuids查询新房楼盘图片信息)

* 真房-SAAS专用-状态查询
    * [消息(员工绑定 楼盘匹配失败)推送规范](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E7%9C%9F%E6%88%BF-%E6%B6%88%E6%81%AF(%E5%91%98%E5%B7%A5%E7%BB%91%E5%AE%9A-%E6%A5%BC%E7%9B%98%E5%8C%B9%E9%85%8D%E5%A4%B1%E8%B4%A5)%E6%8E%A8%E9%80%81%E8%A7%84%E8%8C%83)
    * [获取员工待绑定状态](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/获取员工待绑定状态)
    * [获取楼盘待绑定数量](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/获取楼盘待绑定数量)
    
* 真房-SAAS专用-二手房
    * [批量发送角色人信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量发送角色人信息)
    * [批量发送成交记录](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量发送成交记录)
    * [批量发送带看记录](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/批量发送带看信息)
    
* 58相关
    * [查询58公司token相关信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/查询58公司token相关信息)
    * [58clientId及clientSecret获取58业务token(待废弃)](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/58clientId及clientSecret获取58业务token)
    * [经纪人三网Id获取经纪人巧房公司uuid及员工uuid(电话平台)](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/经纪人三网Id获取经纪人巧房公司uuid及员工uuid)
    * [巧房公司uuid查询58网络门店clientId信息(电话平台)](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/巧房公司uuid查询58网络门店clientId信息)

* 采房
    * [查询区域下的板块](https://github.com/qiaofangyun/qf-housingacquisition/wiki/%E5%9F%8E%E5%B8%82%E8%8E%B7%E5%8F%96%E5%8C%BA%E5%9F%9F)
    * [根据城市获取区域](https://github.com/qiaofangyun/qf-housingacquisition/wiki/%E6%9F%A5%E8%AF%A2%E5%8C%BA%E5%9F%9F%E4%B8%8B%E7%9A%84%E6%9D%BF%E5%9D%97)
    * [查询出售列表](https://github.com/qiaofangyun/qf-housingacquisition/wiki/%E5%87%BA%E5%94%AE%E6%88%BF%E6%BA%90%E8%AF%A6%E6%83%85%E5%88%97%E8%A1%A8)
    * [查询出售详情](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E6%A0%B9%E6%8D%AE%E5%87%BA%E5%94%AE%E6%88%BF%E6%BA%90id%E5%88%97%E8%A1%A8%E8%8E%B7%E5%8F%96%E8%AF%A6%E6%83%85%E6%8E%A5%E5%8F%A3)
    * [查询出租列表](https://github.com/qiaofangyun/qf-housingacquisition/wiki/%E5%87%BA%E7%A7%9F%E6%88%BF%E6%BA%90%E8%AF%A6%E6%83%85%E5%88%97%E8%A1%A8)
    * [查询出租详情](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E6%A0%B9%E6%8D%AE%E5%87%BA%E7%A7%9F%E6%88%BF%E6%BA%90id%E5%88%97%E8%A1%A8%E8%8E%B7%E5%8F%96%E8%AF%A6%E6%83%85%E6%8E%A5%E5%8F%A3)
    * [一键秒入导入回调](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E4%B8%80%E9%94%AE%E7%A7%92%E5%BD%95%E5%AF%BC%E5%85%A5%E5%9B%9E%E8%B0%83)
* 微门店
    * [导入微门店客源](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E5%BE%AE%E9%97%A8%E5%BA%97-%E5%A4%96%E9%83%A8%E7%B3%BB%E7%BB%9F%E5%AF%BC%E5%85%A5%E5%BE%AE%E9%97%A8%E5%BA%97%E5%AE%A2%E6%BA%90%E6%88%90%E5%8A%9F%E5%9B%9E%E8%B0%83%E8%90%A5%E9%94%80%E7%B3%BB%E7%BB%9F)
    * [获取客源信息](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E5%BE%AE%E9%97%A8%E5%BA%97-%E5%A4%96%E9%83%A8%E7%B3%BB%E7%BB%9F%E5%9F%BA%E4%BA%8E%E5%BE%AE%E9%97%A8%E5%BA%97%E5%AE%A2%E6%BA%90uuid%E8%8E%B7%E5%8F%96%E5%AE%A2%E6%BA%90%E4%BF%A1%E6%81%AF)
    * [获取公司的房源名片](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E8%8E%B7%E5%8F%96%E5%BE%AE%E9%97%A8%E5%BA%97%E4%BC%81%E4%B8%9A%E7%9A%84%E6%88%BF%E6%BA%90%E5%90%8D%E7%89%87)
    * [获取scene对应的小程序码](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E8%8E%B7%E5%8F%96scene%E5%AF%B9%E5%BA%94%E7%9A%84%E5%B0%8F%E7%A8%8B%E5%BA%8F%E7%A0%81)
    * [获取微门店企业的新房楼盘名片](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/获取微门店企业的新房楼盘名片)

* Atool
    * [分享房源获取小程序码](https://github.com/qiaofangyun/qf-marketing-openApi/wiki/%E5%88%86%E4%BA%AB%E6%88%BF%E6%BA%90%E8%8E%B7%E5%8F%96%E5%B0%8F%E7%A8%8B%E5%BA%8F%E7%A0%81)



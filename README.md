<h1 align="center">woocommerce - 藍新定期定額外掛</h1>

### 必須安裝之外掛
<table>
    <tr>
        <td>名稱</td>
        <td>版本</td>
        <td>作用</td>
        <td>網站介紹</td>
    </tr>
    <tr>
        <td>woocommerce subscription</td>
        <td>v1.2.1</td>
        <td>搭配 woocommerce 可以使用訂閱制商品</td>
        <td>https://docs.woocommerce.com/document/subscriptions/</td>
    </tr>
    <tr>
        <td>Payment Gateways per Products for WooCommerce</td>
        <td>v1.2.1</td>
        <td>可以針對商品指定付款方式</td>
        <td>https://wordpress.org/plugins/payment-gateways-per-product-categories-for-woocommerce/</td>
    </tr>
</table>

# 啟動步驟
## 安裝外掛
* 安裝 woocommerce subscription 外掛
* 安裝藍新金流定期定額外掛
* 安裝 Payment Gateways per Products for WooCommerce 外掛

## 設定 woocommerce subscription
* Woocommerce -> 設定 -> Subscriptions
    * Manual Renewal Payments
        * 勾選 Accept Manual Renewals
        * 勾選 Turn off Automatic Payments
    * Auto Renewal Toggle
        * Display the auto renewal toggle 
        
## 設定藍新金流定期定額
* Woocommerce -> 設定 -> 付款 -> 藍新金流定期定額 -> 管理
    * 依據需求設定相關參數
    
## 設定訂閱制商品
* 目的

* 商品 -> 新增
    * 商品資料
        * 選取 Simple subscription
            * 一般
                * 設定商品金額
                * 設定商品訂閱制(EX:週、月、年)
                * 設定商品到期時間(EX:幾週後會過期)
            * 庫存
                * 勾選「限購一件」
            * 進階
                * Limit subscription 選擇 「 Limit to one active subscription 」
         * 自行設定 __商品分類__ 或是 __商品標籤__，一定要設定分類或標籤，才能使 __Payment Gateways per Products for WooCommerce__ 有作用。
    * 再來就是依據需求自行設定商品之相關參數(EX: 商品名稱、商品內文、商品發佈..等等)
    

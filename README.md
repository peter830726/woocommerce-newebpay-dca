<h1 align="center">woocommerce - 藍新定期定額外掛</h1>

### 必須安裝之相依外掛
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

## 外掛安裝流程
<ol>
<li>安裝 woocommerce subscription 外掛</li>
<li>安裝藍新金流定期定額外掛</li>
<li>安裝 Payment Gateways per Products for WooCommerce 外掛</li>
</ol>

# 訂閱制設定
* ## woocommerce subscription 設定
    * ### 操作
        * Woocommerce -> 設定 -> Subscriptions
            * Manual Renewal Payments
                * 勾選 Accept Manual Renewals
                * 勾選 Turn off Automatic Payments
            * 其餘選項不要勾選，可能會影響到藍新定期定額模組之運作。
        
* ## 藍新金流定期定額設定
    * ### 操作
        * Woocommerce -> 設定 -> 付款 -> 藍新金流定期定額 -> 管理
            * 依據需求設定相關參數
    
* ## 訂閱制商品設定
    * ### 訂閱制商品與非訂閱制商品需分類
        * 分類的目的在於分開付款方式，使 __Payment Gateways per Products for WooCommerce外掛__ 可以針對商品指定付款方式。
         * 如何才能分類
            * 使用 __商品分類__ 或是 __商品標籤__，兩種分類方式擇一使用即可。
        * 最少需分兩類
            * 訂閱制商品 => 使用 __藍新金流定期定額__ 之付款方式
            * 非訂閱制商品 => 使用 __非藍新金流定期定額__ 之付款方式
    * ### 操作
        * 商品 -> 新增
            * 商品資料
                * 選取 Simple subscription
                    * 一般
                        * 設定商品金額
                        * 設定商品訂閱制(EX:一週扣款一次、一個月扣款一次、一年扣款一次)
                        * 設定商品到期時間(EX:幾個月後會過期)
                    * 庫存
                        * 勾選「限購一件」
                    * 進階
                        * Limit subscription 選擇 「 Limit to one active subscription 」
                 * 商品分類、商品標籤二擇一 
                    - 商品分類：至少分兩類(訂閱制商品、非訂閱制商品)
                    - 商品標籤：至少分兩類(訂閱制商品、非訂閱制商品)
            * 再來就是依據需求自行設定商品之相關參數(EX: 商品名稱、商品內文、商品發佈..等等)


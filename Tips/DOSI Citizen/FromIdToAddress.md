# 從使用者 ID 到使用者地址
* 目前要找使用者的地址有兩種方法
  1. **F12 法**，這方法需要該玩家有夠多的 NFT 才能找到地址
  2. **鏈上搜尋法**，看該使用者有什麼 NFT，然後根據 NFT 去鏈上找他的地址

---

## F12 法
* 如果點開網址後發現他的 NFT 數量大於 20 個，那麼這方法就可以使用，如果比較少的話，請用另一個方法
  * 網址 1：https://citizen.store.dosi.world/zh-TW/profile/90078
    * 數量超過 20 個
  * 範例 2：https://citizen.store.dosi.world/zh-TW/profile/4890720
    * 數量少於 20 個
* 點開網址，然後打開開發者工具(F12)，然後重新整理頁面
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/b63bc19f-23c3-40db-9c29-77adcf1358ee)
* 網頁往下滑直到網頁 load 出大於 20 張 NFT
* 接著回去看網路的頁面，找到一個請求是 collections...，點下去
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/bd62591e-415b-4e83-a7e6-54ddc2697040)
* 到回應的頁面那邊，你會看到下面的畫面
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/8a6ede56-aad4-443c-8b22-87a29356cf20)
* 我們放大看清楚一點 responseData 的資料
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/4025beb6-e962-4f48-9733-737d9d6f140b)
* **address 後面那一串就是這個帳號的地址**，也就是 `link17plxh8650nxkcfhhnnxp74jjfcxyp4hdwksjgx`


## 鏈上搜尋法
* 點開網址 2 或是其他帳號，你會看到他一定有一張 NFT (因為帳號內 NFT 賣不完)
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/523d7fae-cb8f-4360-81f2-909ba1b8ea2f)
* 點進那一張 NFT，找到代幣詳細資訊，圖內的值是 `10000009001133c0`
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/50e5b14a-8982-40c9-92c8-9153f4ed4ded)
* 接著在這網址後面 https://explorer.blockchain.line.me/finschia/item-token/f68e7fd5/ 補上上面的值，像是下面這樣
  * https://explorer.blockchain.line.me/finschia/item-token/f68e7fd5/10000009001133c0
* 打開網址後，點到 Holder 的頁面，上面顯示的地址就是這個帳號的地址，在這範例是 `link1v3jqkcpg6l5hajpgxm2kud4un0t563gar0v7sq`
  ![image](https://github.com/0xygen77/0xygen77.github.io/assets/125109141/32862c8f-6d2e-44b0-9269-7d4860bb3b4d)

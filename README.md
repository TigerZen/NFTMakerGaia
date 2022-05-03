# NFTMakerGaia
 Master of NFT creation
 
 
1.設定抽成上限10BNB,達10BNB自動解除抽成
>>>免除高抽成疑慮,下一版本會設定2BNB付費後就免抽成


2.更改tokenURI查詢外連地址,增加中繼介面合約,方便後續抽換
>>>透過中繼合約可替換查詢位址,不用動到母子合約


3.設定抽成金庫合約地址
>>>子合約用戶提款會把20%轉到官方金庫合約,
金庫合約執行提款後,其中的50%轉給質押分享執行地址,
50%直接轉給21角擁有人地址


4.可以關閉合約部署子合約的功能
>>>新增IsGaiaNFTMakerActive()判斷GaiaIsActive是否為true
>>>SetGaiaNFTMakerActive()函數可以更改GaiaIsActive狀態
>>>GaiaCreateNFT函數新增SetGaiaNFTMakerActive()檢查


5.合約擁有者是否可以設定收益人不同
>>>NFT子合約新增_ownertreasury地址變數
>>>為提幣收款人地址,默認為部屬時的合約擁有人
>>>擁有人可以透過setownerTreasury(address newownerTreasury)變更收款人


新NFT Maker合約
0xE7C6145f0e3203C57E6C6639381084797f1AA77E


新部屬的子合約ID 0
0x7c1c85aD1cFA504B5467005948e5566615A5669B
(0.01BNB/Mint)


新部屬的子合約ID 1
0x7FE1b4C138b06435eE3a64b0405772dAC58d2c1C
(0BNB/Mint)

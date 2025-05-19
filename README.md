# link-api

## 實體
- Space - Space是空間的抽像，可以在Space下創建sub Space，可對應不同的業務邏輯。以物業管理系統為例，可以先創建一個對應組職或公司的Space，然後在這個Space下創建不同的物業，再在物業下創建不同的分座，然後是樓層和單位。
- Role - Role是角色的抽像，Role必定屬於Space，以物業管理系統為例子，Role可作為某個單位的住戶，Account可以透過訂閱成為Role。
- Account - Account是帳號，用於鍳權，每個Account可以屬於多個Role。
- SubscriptionTier - 訂閱套餐對應某個Role，有單人訂閱和多人訂閱模式，單人訂閱模式有人訂閱後其他人無法訂閱。用戶可以𨘋過訂閱成為角色。
## 物業管理系統

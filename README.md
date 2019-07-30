# AIHUB-GeekHub-Project

## Data_cleaning
### binary
* host_is_superhost
* host_has_profile_pic
* host_identity_verified
* is_location_exact
* is_business_travel_ready
* instant_bookable
* require_guest_profile_picture
* require_guest_phone_verification
### multiplement
* bed_type : 'Real Bed' = 0, 'Couch' = 1, 'Futon' = 2, 'Airbed' = 3, 'Pull-out Sofa' = 4 (解决办法：df.replace('x', 'y'))
* room_type : 'Entire home/apt' = 0, 'Private room' = 1, 'Shared room' = 2
* cancellation_policy :'strict_14_with_grace_period' = 0, 'moderate' = 1, 'flexible' = 2
### Data-cleaning dairy
* first version, 我们从106列特征通过人工筛选的方式将 与价格没有关系的特征缩减为47列
* second version, 我们将可分类的数据数字化, 将二元t/f换成1/0, 将多元成分也同样以数字的形式呈现。
* third version, 我们根据first review feature 删除了一些数据, 从 31457行 到 18545行, 因为我们认为没有人所观看的房子的价格没有可借鉴的价值
* Fourth version, 我们将host_response_rate中的null值 用剩余值的平均值替换
* Fifth version, 我们将price和 extra_price改为数字格式, 例子（1,000格式改为数字格式 1000）
* 0720_1750 全部内容处理完成（独热码），未进一步drop行。next step : rule : [price <(50 * accomondates)] -> drop
* 0721_2300 保留 ([price > (50 * accomondates)] & [price > (50 * beds]) & [min_nights <= 3])
* 0722_2300 删除了 >2w & 9999的数据, beds < 50, bathrooms = 101.5 -> 1
* 0725_2200 新增房屋距离市中心的距离Distance
* 0729_2200 新增房屋距离最近地铁站的距离subwayDistance
## 遇到的问题
* 如何修改dataframe某一列的问题
## source
  北京地铁经纬度

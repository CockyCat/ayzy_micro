
# 最近更新
2022-07-22 

当鉴权失败时，返回401，跨域的处理不能统一化，不同的Http状态码都可能会存在跨域问题。

Token鉴权失败时，由直接返回Http 401状态码改为返回200，增加Json输出401的状态码，通过此码来识别Token鉴权失败。

跨域时，只处理200的情况即可。

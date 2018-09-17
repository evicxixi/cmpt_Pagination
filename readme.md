# 分页插件 Pagination
~~~
: param current_page: 当前页码
: param per_page: 每页显示数据条数
: param all_count: 数据库中总条数
: param base_url: 基础URL
: param query_params: QueryDict对象，内部含所有当前URL的原条件
: param pager_page_count: 页面上最多显示的页码数量
~~~

## 补充：
query_params部分由于是QueryDict对象，在Django中的QueryDict对象具有urlencode()方法。
若在其它框架中，只要传入的是dict类型数据，可引入模块进行url的转化：
~~~
from urllib.parse import urlencode
~~~

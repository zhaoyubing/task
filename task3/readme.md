字典在数据库中的应用：数据压缩字典的实现。

为part.tbl数据表的P_CONTAINER列建立字典表，为P_CONTAINER列中每个值分配一个字典编码，字典表编码为自然数列。 

生成压缩的P_CONTAINER列，内容为其原始值对应的字典编码。 模拟执行`P_CONTAINER='WRAP BOX'`操作，先在字典表中查找'WRAP BOX'对应的编码，然后在压缩的P_CONTAINER列上执行基于编码值的查找操作，统计满足条件的记录的数量（计数操作）。

对比原始P_CONTAINER列上的`P_CONTAINER='WRAP BOX'`条件计数操作过程，简要说明使用字典表的好处。

**命名格式**：学号-思考题3-姓名

### Repositories目录说明（Repository层）
1. Repository层，所有仓库类放置在该目录下。通常按照业务/数据库进行划分
2. Repository层的职责：
    - 仅包含对数据库直接进行增删改查操作的代码，辅助Model层（除此之外请不要放置其他代码；通常增删改的逻辑比较单一，而查则会有多种情况，将各种查询逻辑在此处实现）
3. Repository层仅包含直接对数据库进行操作的代码，其他涉及外部调用等功能的代码应该考虑放置在Service层中。
4. 所有的仓库类应该继承自AppRepository类

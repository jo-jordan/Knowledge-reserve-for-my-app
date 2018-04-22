> ## RecyclerView
> ### 什么是RecyclerView?
> RecyclerView是ListView的改进版，它可以垂直滚动，水平滚动，还可以是格子，是一个装载着有限数量views的容器，是一种高效的可滚动视图。
> ### RecyclerView的目的在于
> 1. 减少在每次创建view时的调用findViewById()方法的高昂开销，即减少内存占用。这在一定程度上减少了电量的损耗。
> 2. 减少在创建view所花费的时间。

> ### RecyclerView涉及到的组件
> - Data：数据源，不论来源，本地也好，云端也好，假的也罢
> - A RecyclerView：包含list items的可滚动视图
> - Layout for one item of data：RecyclerView中的子项布局定义
> - A layout manager：布局管理器，每个ViewGroup都拥有一个布局管理器([RecyclerView.LayoutManager](https://developer.android.com/reference/android/support/v7/widget/RecyclerView.LayoutManager.html))，它管理着每一个子项的布局
> - An adapter：这里用到的是[RecyclerView.Adapter](https://developer.android.com/reference/android/support/v7/widget/RecyclerView.Adapter.html)将数据与RecyclerView相连接，负责准备数据，当数据发生变化时，它会即时更新视图
> - A view holder：每个ViewHolder([RecyclerView.ViewHolder](https://developer.android.com/reference/android/support/v7/widget/RecyclerView.ViewHolder.html))持有着一个item view的信息

> ### RecyclerView工作原理
> ![image](https://raw.githubusercontent.com/lzjlxebr/Knowledge-reserve-for-my-app/master/images/RecyclerView%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86.png)

# 学习笔记

## Week02 作业题目：
### 1. 我们在数据库操作的时候，比如 dao 层中当遇到一个 sql.ErrNoRows 的时候，是否应该 Wrap 这个 error，抛给上层。为什么，应该怎么做请写出代码？
答： sql.ErrNoRows作为标准库的sentinel Err只标识了错误信息，在dao这一层应该Wrap这个error。

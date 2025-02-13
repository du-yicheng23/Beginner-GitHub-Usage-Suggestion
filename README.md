# Github 新手使用建议

以下建议只是根据作者个人经验总结的，不一定适用于所有情况。若存在错误也请批评指正，谢谢！

1. 对于所有纯文本文件（包括源代码与文档），应当统一使用 `UTF-8(NO BOM)` 文件编码格式，换行符为 `LF`。有关文件编码格式与换行符的说明详见[文档](./中文乱码的原因、%20UTF-8%20的设置以及换行符.md)。
2. 注意缩进是否使用制表符（根据当前项目的规范文档决定，多数情况都是统一使用空格缩进）。
3. 除非你是仓库拥有者或内部开发成员，否则不应当直接把你的修改提交到仓库中。那么对于非仓库内部成员，应当如何贡献代码呢？答案是使用 `Fork` 功能 —— 点击仓库右上角的 `Fork` 按钮，将这个仓库“Fork”（动词）到自己的账号内，这样你自己的账号内就创建了一个新的仓库，如图<br>
![](./_attach/forked-repo-example.jpg)<br>
可以看到，被 Fork 过来的仓库右上角多了两个选项。其中 `Sync Fork` 表示从主仓库拉取提交，也就是说如果原来的仓库发生了修改后，可以通过这个按钮将主仓库的更改拉取到自己账号下的这个 Fork 仓库中，从而实现与主仓库同步。同理，`Contribute` 按钮可以将自己账号下的 Fork 仓库提交的更改推送到主仓库中，这样就可以在不影响到主仓库的情况下贡献代码了。<br>
![](./_attach//fork-repo-pull-request-demo.jpg)<br>
例如此处，在 Fork 仓库中创建了一个新的分支，然后再把更改提交到这个新分支内，这样就可以点击这个按钮创建一个 Pull Request, 从而请求主仓库的管理员将这个提交合并到主分支中。
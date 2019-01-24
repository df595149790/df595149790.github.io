
# 遇到的一个搞笑的问题

在 CLion 中安装 bazel 插件后，按照手册执行，创建工程后，sync 工程，结果总是报告一个错误

Bazel Problems
```text
Error:Cannot run program "bazel" (in directory ".../bazel/examples/cpp-tutorial/stage1"): 
      error=2, No such file or directory
Error:Could not run Bazel info
```

Bazel Console
```text
Syncing project: Sync (incremental)...
Updating VCS...
Running Bazel info...
Command: bazel info --tool_tag=ijwb:CLion --curses=no --color=yes --experimental_ui=no --progress_in_terminal_title=no --


==== TIMING REPORT ====

Sync: 38ms
    BazelInfo: 29ms

Timing summary:

BlazeInvocation: 29ms
Sync failed
```

百思不得其解，也搜索不到答案。碰巧，今天 bing 还无法访问，很郁闷。

后来才发现，CLion 的 Preferences 中的 Bazel Settings 中，Bazel binary location 是缺省值
```text
bazel
```

更改为绝对路径，就OK了
```text
/usr/local/bin/bazel
```

愚蠢的提示信息。




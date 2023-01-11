# mmdetection_modified_tools


## About benchmark-batchsize16.py

The original mmdetection benchmark tools are too slow, due to "sample_per_gpus=1", this problem also mentioned by others: 
[https://github.com/open-mmlab/mmdetection/issues/6937](https://github.com/open-mmlab/mmdetection/issues/6937)

In this issue, wywywy01 said that try batch mode，just set batch size to 8，16 or more [code line](https://github.com/open-mmlab/mmdetection/blob/master/tools/analysis_tools/benchmark.py#L67)

Therefore, I modify tools/analysis_tools/benchmark.py. During the modification process, i encounter a problem about calculating batchsize, the process of solution at 
[https://blog.csdn.net/weixin_42362903/article/details/128640306](https://blog.csdn.net/weixin_42362903/article/details/128640306).

I rename the modified file as "benchmark-batchsize16.py". In this file, i put code annotation on the line above the line of code being modified. 
----"# 修改" means the next few lines code have been modified
----"# 新增" means i add several lines code

# 将/tmp/0829/tmpconf/bash_p 文件中的内容追加到 /data/app/app/.bash_profile文件后面
# ansible rdfa-srv -m shell -a "cat   /tmp/0829/tmpconf/bash_p >> /data/app/app/.bash_profile "
批量复制目录下文件

将/tmp/0829/hdfs/下的文件全部复制到/data/app/app/conf/edw/下面
ansible rdfa-srv -m shell -a "src=/tmp/0829/hdfs/  dest=/data/app/app/conf/edw/"
查看/data/app/app/conf/edw/下面的文件
ansible rdfa-srv -m shell -a “/data/app/app/conf/edw/”

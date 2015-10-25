#一次向svn中增加所有新增文件 svn add all new files
>svn st | awk '{if ( $1 == "?") { print $2}}' | xargs svn add

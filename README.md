# 小王总仓库
Git Submodule 允许一个git仓库，作为另一个git仓库的子目录，并且保持父项目和子项目相互独立。

包含vue、react等模板开发的活动仓库
当前添加了三个分仓库：
>   git submodule add git@gitlab.19ego.cn:largeFrontEndProjects/gy-activities-react.git    
>   git submodule add git@gitlab.19ego.cn:largeFrontEndProjects/gy-activities-vue.git    
>   git submodule add git@gitlab.19ego.cn:largeFrontEndProjects/gy-activities-gulp.git
继续添加分仓库，继续git submodule add即可。
主仓库提交代码不会影响分仓库。
第一次拉取总仓库时，带上递归参数可以同步拉取分仓库。
>   git clone git@gitlab.19ego.cn:largeFrontEndProjects/gy-all-activities.git --recurse-submodules
也可以先拉取总仓库，然后执行命令获取分仓库：
>   git submodule init
>   git submodule update
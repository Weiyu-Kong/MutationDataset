Mutation dataset for Tracerecov experiment.

（第二批仅保留mutate文件的）



- **OriginalProjects** 中为原项目；

- **MutationFiles** 中为mutate出的文件，包含.java和.class，以及记录全限定类名和方法名的failing_tests；

- 由于空间占用问题只保留了mutate针对的文件，使用时可能需要：

    - 复制原项目到某个工作目录，作为fix版本，并再复制一份作为bug版本；
    - 根据failing_tests中记录的全限定类名，找到mutate后的源文件和目标文件在项目中的位置，分别替换为mutate后的版本；
    - 将failing_tests移动到bug目录中。

    


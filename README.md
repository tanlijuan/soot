# soot的使用方法：
在Linux系统中，切换到Java项目中，你要生成控制流图的那个类的目录下，然后输入指令：
java -cp soot-2.5.0.jar soot.tools.CFGViewer --soot-classpath .:/usr/jdk1.7.0_79/jre/lib/rt.jar Triangle
说明：.:/usr/jdk1.7.0_79是你当前系统所装jdk的目录，Triangle是你要生成控制流图的类。
然后会生成一个sootOutput文件夹，会有.dot文件。
然后切换到sootOutput目录下，输入指令：
dot -Tpng Triangle.dot -o Triangle.png
书名：Triangle.dot是sootOutput文件夹中.dot文件改名之后的，Triangle.png是生成的控制流图


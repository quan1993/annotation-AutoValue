# annotation-AutoValue
AutoValue的使用方法及作用

AutoValue是代码生成器，可以帮助我们减少代码的编写。

使用之前需要在pom.xml文件中添加依赖
<dependency>
			<groupId>com.google.auto.value</groupId>
			<artifactId>auto-value</artifactId>
			<version>1.2</version>
		</dependency>

建立抽象类（包含自己需要调用的抽象方法）
  如Complex.java
（现在这个类是错误的，因为AutoValue_Complex这个类还不存在）

编译Complex.java所在的项目，生成jar包
（编译方法：项目右击--run as--run as configurations--maven ）

再在该项目中添加对该jar包的依赖（直接在pom.xml文件中添加依赖，可能不成功，就需要build path手动添加该jar包）

之后Complex.java就不报错了，我们也可以查看生成的AutoValue_Complex.class文件

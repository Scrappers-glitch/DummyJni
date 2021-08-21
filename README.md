# DummyJni

### Commands to Compile : 
```bash
┌─[twisted@parrot]─[~/GradleProjects/DummyJni]
└──╼ $javac -h . TestJni.java 
┌─[twisted@parrot]─[~/GradleProjects/DummyJni]
└──╼ $   gcc -fPIC 'TestJni.cpp' -shared  -o 'libTestJni.so' \
>                 -I'/usr/lib/jvm/java-11-openjdk-amd64/include' \
>                 -I'/usr/lib/jvm/java-11-openjdk-amd64/include/linux' \
>                 -I${workDir}'/code/natives/includes'
┌─[twisted@parrot]─[~/GradleProjects/DummyJni]
└──╼ $java -cp . -Djava.library.path=. TestJni
hey
┌─[twisted@parrot]─[~/GradleProjects/DummyJni]
└──╼ $
```

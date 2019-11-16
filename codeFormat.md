 ### 代码格式/规范
 良好的代码格式和规范，易于维护，也更容易暴露出潜在的问题
 
```
//A
 public class App 
{
    public static void main( String[] args )
    {
        Long o = null;
        if(args != null){
            o = 1L;
        }
        for(int i=0;i<2;i++) {
            if (o != null) {
                System.out.println("hello");
            } else {
                System.out.println("world");
            }
        }

    }
}
```
```
//B
public class Bpp {

    public static void main(String[] args) {
        Long o = null;
        if (args != null) {
            o = 1L;
        }
        for (int i = 0; i < 2; i++) {
            if (o != null) {
                System.out.println("hello");
                continue;
            }
            System.out.println("world");

        }

    }
}
```
对于A和B这两份代码格式，倾向于B。
在执行效率方面，两份编译后，通过反编译查看，发现编译后的字节码是一样的

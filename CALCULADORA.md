## Calculadora - simples                            

fun main () {
**val** x:Int; <br/>
**val** y:Int; <br/>
**val** z:Int; <br/>
**val** w:Int; <br/>

    x = calculate(8 , 5, ::sum)
    y = calculate(9 , 6){a,b -> a*b}
    z = calculate(100 , 63){a,b -> a-b}
    w = calculate(280, 2){a,b -> a/b}
    
    println(x)
    println(y)
    println(z)
    println(w)

} <br/>
**fun** sum(x1:Int,x2:Int) = x1.plus(x2) <br/>
**fun** mul(y1:Int,y2:Int) = y1.times(y2) <br/>
**fun** sub(z1:Int,z2:Int) = z1.minus(z2) <br/>
**fun** div(w1:Int,w2:Int) = w1.div(w2) <br/>

**fun** calculate(n1:Int, n2:Int,operation:(Int,Int)->Int):Int{ <br/>
    **val** result = operation(n1,n2) <br/>
    **return** result <br/>
    } <br/>
    

**13;** <br/>
**54;** <br/>
**37;** <br/>
**140;** <br/>


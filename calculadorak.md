## Calculadora - simples                            

<p>fun main () {</p>
<p>**val** x:Int; </p>
<p>**val** y:Int;</p> 
<p>**val** z:Int; </p>
<p>**val** w:Int</p>

    x = calculate(8 , 5, ::sum)
    y = calculate(9 , 6){a,b -> a*b}
    z = calculate(100 , 63){a,b -> a-b}
    w = calculate(280, 2){a,b -> a/b}
    
    println(x)
    println(y)
    println(z)
    println(w)

}
**fun** sum(x1:Int,x2:Int) = x1.plus(x2)
**fun** mul(y1:Int,y2:Int) = y1.times(y2)
**fun** sub(z1:Int,z2:Int) = z1.minus(z2)
**fun** div(w1:Int,w2:Int) = w1.div(w2)

**fun** calculate(n1:Int, n2:Int,operation:(Int,Int)->Int):Int{
    **val** result = operation(n1,n2)
    **return** result
    }
    

**13**
**54**
**37**
**140**


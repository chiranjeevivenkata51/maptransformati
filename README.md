# maptransformati
Data:
101,Amar,40000,m,11
102,Chiru,50000,M,12
103,MAni,58000,f,15
104,VenkaTa,53000,F,18
105,SAi,58000,,m,11
 
TRANSFORMATION                                      1st iteration
val c = l.map{a=>                                   101,Amar,40000,m,11 
val b =a.split(",")                      //Intimating the compiler that divide the array by "," delimiter   
                                          b(0)=101 b(1)=Amar,b(2)=40000,b(3)=m,b(4)=1
val wc = b(1).substring(0,1).toUpperCase  //
val cn = b(1).substring(1,b(1).size).toLowerCase
var e = b(2).toInt * 10/100
var f = b(2).toInt * 20/100
val n = b(2).toInt + f - e
val cs = b(3).toLowerCase
val df = if (cs == "m") "Male" else "Female"
((wc+cn),e.toInt,f.toInt,f.toInt,n.toInt,df)
}

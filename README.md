# Firstrepo
 Demo
package com.positiveedge

object MonomorphicArray extends App {
  var data: Array[String] = Array("java","python","scala","c#","c",".net","scala","c++","scala");
  var count: Int =0;
  def f1(value:String): Unit = {
  {
    for (i  <- 0 to (data.length-1))
    {
      if(data(i)==value)
        {
          count =count+1;
        }
    }
  }
  if (count == 1)
    {
      println("It is monomorphic array string")
    }
  else
    {
      println("It is not a monomorhic array")
    }
  }
  f1("java")


  // polymorhic elements


  def f2(): Unit ={

    for(i <- 0 to data.length-1)
      {
        for(j <- i+1 to data.length-1)
          {
            if(data(i) == data(j))
              {
                println(data(i))
              }
          }
      }
  }

    f2()

}

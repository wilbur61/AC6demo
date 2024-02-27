# AC6demo
AC6demo
Guided Lab - 309.5.5 - SP7 - How to use @RequestParam annotation

Objective:
In this lab, we will demonstrate how to use @RequestParam annotation. By the end of this lab, learners will be able to utilize the @RequestParam annotation.

Concept Revision: 
The @RequestParam annotation binds a web request parameter (i.e., query string) to a method parameter in a controller.
The following code snippet shows the usage of the @RequestParam annotation.


Request URL with a query string:
http://localhost:8080/request1?name=David
Accessing value of name parameter in handler method:
@RequestMapping("/request1")
public String handler(@RequestParam(name = "name") String name) {
…  }

Let’s see a complete example of how to use the @RequestParam annotation to bind request parameters to method parameters in a controller.

# Run and Test
Type the following URLs in the browser's address bar and see the output.
 1- http://localhost:8080/request1?name=David%20Miller
 2- http://localhost:8080/request2?firstName=David&lastName=Miller
 3 - http://localhost:8080/request3?name=David&age=32&amount=1200.50&active=1
 4 -http://localhost:8080/request4?name=David&age=32&country=USA&city=NewYork
 5 - http://localhost:8080/request5?firstName=David&lastName=Miller
 6 - http://localhost:8080/request6?date=2017-12-12&time=12:54:52
 7-http://localhost:8080/request7?country=USA&country=PAKISTAN&country=Japan&city=NYC&city=KARACHI&city=TOKYO
 8 - http://localhost:8080/request8

 

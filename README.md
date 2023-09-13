Data transfer in angular:


1. parent to child
-using input decorator (@input).
-using view child (@viewChild).

2. child to parent
-using output decorator (@output).

3. using services + observable.

4. state management.
















@input decorator –:
1.declare @input decorator variable in child .
2.use string interpolation to display in child .

![image](https://github.com/Darpan10/login-crud/assets/49149019/2e53c404-cd93-4dd8-8932-ff43cd18c487)


 

3. in parent component :
Inside [message] is the variable of child component that is binded with “message” of parent component.
 ![image](https://github.com/Darpan10/login-crud/assets/49149019/fb86979c-dac5-450e-89ce-3a935d358fcf)

Conclusion: in the context of Angular, the @Input() decorator is used to declare input properties for child components, allowing data to flow from parent components to child components.
In the parent component's template, you can bind a value to the input property of the child.
























@output –:
![image](https://github.com/Darpan10/login-crud/assets/49149019/82690e19-31f7-4125-b21b-1e0cdb18a391)

 
1.create a variable in child component called message 
2.declare event emitter 
3.inside a function sendMessage() emit the message.
4.create a button to trigger sendMessage() in html.
 ![image](https://github.com/Darpan10/login-crud/assets/49149019/5818ffd7-9852-42fd-bcae-db8ef425b20c)


5.emit from app-child component so that the emitter emitted the event from the child component entirely <app-child> and parent component will listen to it.
6.(messagevent) is child binded component used <app-child>
7. in parent component create recieveMessage($event) to receive the message 
8.declare event with this.message.
9. display with string interpolation {{message}}.




Viewchild :
 


![image](https://github.com/Darpan10/login-crud/assets/49149019/b5d37479-5800-4e50-9e0a-28c08be289fc)



notes : 

use ngmodel,ngform directive to bind input form value and 
provide validation as well. for template driven form


















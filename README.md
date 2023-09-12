![image](https://github.com/Darpan10/login-crud/assets/49149019/cc97af6c-ac5c-45b3-8bd4-64c7b66065c2)Data transfer in angular:


1. parent to child
-using input decorator (@input).
-using view child (@viewChild).

2. child to parent
-using output decorator (@output).

3. using services + observable.

4. state management.










![image](https://github.com/Darpan10/login-crud/assets/49149019/df77e844-4b28-432b-b1da-755edae8111a)






@input decorator –:
1.declare @input decorator variable in child .
2.use string interpolation to display in child .



 

3. in parent component :
Inside [message] is the variable of child component that is binded with “message” of parent component.
 
Conclusion: in the context of Angular, the @Input() decorator is used to declare input properties for child components, allowing data to flow from parent components to child components.
In the parent component's template, you can bind a value to the input property of the child.
























@output –:
 
1.create a variable in child component called message 
2.declare event emitter 
3.inside a function sendMessage() emit the message.
4.create a button to trigger sendMessage() in html.
 

5.emit from app-child component so that the emitter emitted the event from the child component entirely <app-child> and parent component will listen to it.
6.(messagevent) is child binded component used <app-child>
7. in parent component create recieveMessage($event) to receive the message 
8.declare event with this.message.
9. display with string interpolation {{message}}.




Viewchild :
 






















